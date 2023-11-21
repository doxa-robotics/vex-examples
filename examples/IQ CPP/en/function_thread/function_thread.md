category: functions  
signature: function_thread
description: Allows you to execute multiple threads at the same time.

# Thread

Allows you to execute multiple threads at the same time.

```cpp
thread myThread = thread(myThreadCallback);
```

## How To Use

A function needs to be defined that will be passed as a callback to the thread.

```cpp
void myThreadCallback() {
  Brain.Screen.print("In a different thread!");
}
```
Once you have the function written, you can use it to make a new thread. This function is referred to as the **callback function**.

```cpp
thread myThread = thread(myThreadCallback);
```
The **thread** will start executing once it is created. It will then run at the same time as the main thread.

Only **2 threads** should be running at a given time. Additional threads may reduce the performance of the VEX IQ robot.
    
## Example

This example will print two counters to the VEX IQ's Brain at the same time. One will be printed by the `myThread` thread. The other will be printed by the main thread at the same time.

```cpp
void myThreadCallback() {
  int count = 0;
  while(true) {
    Brain.Screen.setCursor(1, 1);
    Brain.Screen.print("thread1: %d", count);
    count++;
    // Wait to allow the main thread to execute
    wait(25, msec);
  }
}

int main() {
  // Once a thread is created it begins executing
  thread myThread = thread(myThreadCallback);
  
  int count = 0;
  while(true) {
    Brain.Screen.setCursor(2, 1);
    Brain.Screen.print("main: %d", count);
    count++;
    // Wait to allow myThread to execute
    wait(25, msec);
  }
}
```

<advanced>
</advanced>
