# isolateexample

Flutter applications are single-threaded applications; this single thread is also called the "main()" thread. You can find this main() thread in the "main.dart" file.
Now the problem is that if you use this single thread for multiple tasks like UI rendering, API calls, State-management, and Business logic, then you will see some micro stutter in your application. This stuttering or drop frame is mostly observed while running animations like app drawer, drop-down menu, pop-up dialog, etc. The solution for this problem is to use a separate thread for executing heavy tasks. Hence the multi-threading implementation comes.
In flutter, there is a class called "Isolate", which executes any tasks isolated from the main thread. You can read more about this Isolate class from this URL: https://api.dart.dev/.../dart-isolate/Isolate-class.html
