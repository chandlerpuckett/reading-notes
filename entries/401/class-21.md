# Tasks and the Back Stack

> A task is a collection of activities that users interact with when performing a certain job. The activities are arranged in a stack—the back stack)

- When Activity A starts Activity B, Activity A is stopped, but the system retains its state (such as scroll position and text entered into forms). If the user presses the `Back` button while in Activity B, Activity A resumes with its state restored

- When the user leaves a task by pressing the `Home` button, the current activity is stopped and its task goes into the background. The system retains the state of every activity in the task. If the user later resumes the task by selecting the launcher icon that began the task, the task comes to the foreground and resumes the activity at the top of the stack.

- If the user presses the `Back` button, the current activity is popped from the stack and destroyed. The previous activity in the stack is resumed. When an activity is destroyed, the system does not retain the activity's state.

- Activities can be instantiated multiple times, even from other tasks.


### Managing Tasks
> The way Android manages tasks and the back stack, as described above—by placing all activities started in succession in the same task and in a "last in, first out" stack

the principal `<activity>` attributes you can use are:
1. `taskAffinity`
2. `launchMode`
3. `allowTaskReparenting`
4. `clearTaskOnLaunch`
5. `alwaysRetainTaskState`
6. `finishOnTaskLaunch`

the principal intent flags you can use are:
1. `FLAG_ACTIVITY_NEW_TASK`
2. `FLAG_ACTIVITY_CLEAR_TOP`
3. `FLAG_ACTIVITY_SINGLE_TOP`

# Android SharedPrefences
> If you have a relatively small collection of key-values that you'd like to save, you should use the SharedPreferences APIs

- A SharedPreferences object points to a file containing key-value pairs and provides simple methods to read and write them
- Each SharedPreferences file is managed by the framework and can be **private** or **shared** 