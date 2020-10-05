# Spring Authentication

- The main strategy interface for authentication is `AuthenticationManager` which only has one method:

> `Authentication authenticate(Authentication authentication) 
  throws AuthenticationException;`


An AuthenticationManager can do one of 3 things in its authenticate() method:

1. return an `Authentication` (normally with authenticated=true) if it can verify that the input represents a valid principal.

2. throw an `AuthenticationException` if it believes that the input represents an invalid principal.

3. return `null` if it can’t decide.


`AuthenticationException` is a runtime exception. It is usually handled by an application in a generic way, depending on the style or purpose of the application


# Spring Auth CheatSheet

## Step 1: set up a user model and repo

## Step 2: create a controller for that model

## Step 3: UserDetailsServiceImpl implements UserDetailsService

gets a User from the database by username (make sure your repository has the method to make this easy!)

## Step 4: ApplicationUser implements UserDetails

use IntelliJ to implement the methods; make the boolean ones all return true

## Step 5: WebSecurityConfig extends WebSecurityConfigurerAdapter

- has a UserDetailsService
- passwordEncoder bean
- configure AuthManagerBuilder
    - `auth.userDetailsService(userDetailsService).passwordEncoder(passwordEncoder());`
- configure HttpSecurity
    - cors? csrf?
    - matchers for URLs that are allowed
        - ensure that login and signup URLs allowed; also consider homepage etc.
    - formLogin with login page set up
    - logout

```
    @Override
    @Bean
    public AuthenticationManager authenticationManagerBean() throws Exception {
        return super.authenticationManagerBean();
    }
```

## Step 6: registration page
- create it w/ form
- ensure it posts to a route your controller is ready for
- check it's saving in the DB
```
    // maybe autologin?
    Authentication authentication = new UsernamePasswordAuthenticationToken(newUser, null, new ArrayList<>());
    SecurityContextHolder.getContext().setAuthentication(authentication);
```

## Step 7: login page
- create it w/ form
- ensure it posts to the route you specified in web config
- try it out!
- add to a template w/ things about the Principal