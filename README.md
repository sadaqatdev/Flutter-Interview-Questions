Flutter is a new platform that everyone is still learning that is why most of the devs not able to find what to prepare for Flutter interview. This blog is helpful for both interviewer and candidate.

<img src="images/flutter_interview.png" height="400" alt="Profile image"/> 

Following are the types of questions asked in the interview.
1. Life Cycle & Routes
2. Widgets
3. Async operations
4. Storage
5. Platform Specific Android/iOS
6. Dart
7. Architecture
8. Test Cases

some also related to assets, firebase, etc…

# 1. Life Cycle & Routes
- Why Flutter? over other platforms?

  flutter is frame work under the hood it use the c++ impler rendering engine and the dart and flutter which compile into native biniry for each platform this enables 60 fps speed , its widget and declarive UI and hotreold feature make development speed.
    
- What is a Widget in Flutter? Why Flutter doesn’t have other files like XML, styles, etc…?
- Difference between a StatelessWidget and a StatefulWidget in Flutter?
- Explain the Stateful Widget Lifecycle?
- How Flutter Lifecycle different from the Android/iOS life cycle?
- How build() method works? How it rebuild itself?
- Does a new state object is created if the widget re-build?
- What is a Navigator and what are Routes in Flutter?
- What are the trees available in Flutter? Eg: Widget Tree, Element Tree…
- What is the ephemeral state? and Differentiate between ephemeral state and app state? [Learn from here](https://flutter.dev/docs/development/data-and-backend/state-mgmt/ephemeral-vs-app)
- When do we use the WidgetsBindingObserver?
- Difference between SchedulerBinding and WidgetBinding? [Learn from here](https://medium.com/flutterworld/flutter-schedulerbinding-vs-widgetsbinding-149c71cb607f)
- How would you access StatefulWidget properties from its State?
- If the child widget gets re-initialized, does it also re-initialize the parent widget?
- How to re-initialize parent widget from child widget? Explain several ways?
# 2. Widgets
- What would happen if I converted a stateless widget to Stateful Widget? Is there any performance issue?
- Flexible Vs Expanded [Learn from here](https://stackoverflow.com/questions/52645944/flutter-expanded-vs-flexible)
- SizeBox VS Container?
- What is a Spacer widget?
- How to show/hide widgets? [Learn from here](https://stackoverflow.com/questions/44489804/show-hide-widgets-in-flutter-programmatically)
- What is the importance of a TextEditingController?
- How to shift focus to next TextField in flutter? [Learn from here](https://stackoverflow.com/questions/49410975/changing-focus-from-one-text-field-to-the-next-in-flutter/62709652#62709652)
- List the Visibility widgets in flutter and the differences?
- What are the ways to get data from called Widget?
- Why ListView inside Column not works?
- Differentiate between Listview and Listview.Builder? [Learn from here](https://stackoverflow.com/a/63075581/5106574)
- How to scroll to a position in Flutter ListView?
- How to place a listview inside a SingleChildScrollView but prevent them from scrolling separately? [Learn from here](https://stackoverflow.com/a/63080296/5106574)
- How can you update a ListView dynamically?
- When to use ShrinkWrap the property?
- Why do we use a Reverse property in a Listview?
- What is an UnmodifiableListView?
- What is SliverList and how to use it?
- How to draw Text over Image? [Learn from here](https://medium.com/flutterworld/flutter-text-over-image-bb045a129bae)
- What are keys in Flutter and when should you use them?
- What are GlobalKeys?
- When should you use mainAxisAlignment and crossAxisAlignment?
- When can you use double.INFINITY?
- When to use a mainAxisSize? and diff between MainAxisSize.min andMainAxisSize.max ?
- What is the purpose of a SafeArea?
    - SafeArea is basically a glorified Padding widget. If you wrap another widget with SafeArea, it adds any necessary padding needed to keep your widget from being blocked by the system status bar, notches, holes, rounded corners, and other "creative" features by manufacturers.
```dart
SafeArea(
  minimum: const EdgeInsets.all(16.0),
  child: Text('My Widget: ...'),
)
```
- How to assign min-height to the widget? [Learn from here](https://stackoverflow.com/questions/48675781/flutter-correct-way-to-create-a-box-that-starts-at-minheight-grows-to-maxheig/62896724#62896724)
- How to align two items on extremes - one on the left and one on the right? [Learn from here](https://stackoverflow.com/questions/50365770/flutter-align-two-items-on-extremes-one-on-the-left-and-one-on-the-right)
- Mention two or more operations that would require you to use or return a Future.
- Can we use Color and Decoration property simultaneously in the Container? Explain
- In order for the CrossAxisAlignment.baseline to work what is another property that we need to set?
- When should we use a resizeToAvoidBottomInset?
- Difference between a Modal and Persistent BottomSheet with an example?
- How is an Inherited Widget different from a Provider?
- What is an InheritedWidget? List some examples.
- When to use Intrinsic height?
- When to use Custom ScrollView?
- Difference between GestureDetector and InkWell? [Learn from here](https://stackoverflow.com/questions/43692923/flutter-container-onpressed/62310664#62310664)
- What is a vsync?
- Difference between AnimationController and Animation?
- When to use a SingleTickerProviderStateMixin and TickerProviderStateMixin?
- What is Ticker, Tween and AnimatedBuilder?
- What is an AspectRatio widget used for?
- What is the purpose of ModalRoute.of()?
- Difference between RemoveUtil and PopUtil in Flutter navigation? [Learn from here](https://stackoverflow.com/questions/62710395/difference-between-removeuntil-and-popuntil-in-flutter-navigation/62711118#62711118)
- Difference between a Navigator.pushNamed and Navigator.pushReplacementNamed?
- What is the use of WidgetsBinding class?
- How to perform Hero Animation?
- Difference between Element Tree, Widget Tree and Render Tree.
- How to get responsive Flutter layouts? [Learn from here](https://stackoverflow.com/questions/59976971/how-to-get-responsive-flutter-layouts)
   
# 3. Async operations
- Explain async, await , thenand Future keyword
- Use of yeild keyword?
- Why build re-triggering again and again? How to scroll to a position in Flutter ListView?
- Why FutureBuildercalled multiple times? how to resolve this? [Learn from here](https://stackoverflow.com/questions/57793479/flutter-futurebuilder-gets-constantly-called/63299888#63299888)
- What's the difference between async and async* in Dart?
- What is a Stream?
- Differentiate between StreamBuilder and FutureBuilder
- What is the difference between FutureBuilder and await?
- What are the ways to use Future Object?
- How to group multiple Streams?
- Why await is not blocking UI? [Learn from here](https://stackoverflow.com/questions/62823273/why-in-this-code-await-is-not-blocking-ui-in-flutter/62823966#62823966)
- How to perform Syncrnonization in Flutter? [Learn from here](https://stackoverflow.com/questions/63176601/flutter-dart-how-to-perform-synchronization/63176650#63176650)
- Differentiate between Provider and Consumer? [Learn from here](https://stackoverflow.com/a/61820608/5106574) 
- How to run foreground services?
- How to schedule a job after specific intervals?
- Difference between whenCompleted() and then().
- How to run code after Build() method execution?
- How to create an HTTP client with headers?
```dart
/// To get it done, we need one endpoint and headers and make the HTTP request.

import 'package:http/http.dart' as http;
final url = Constants.BASE_URL + 'endpoint';
final headers = {'Content-Type': 'application/x-www-form-urlencoded'};//if required
Response getResponse = await http.get(Uri.parse(url), headers: headers);
int statusCode = getResponse.statusCode;
String responseBody = getResponse.body;
print('response----' + responseBody);

```
- Use of http and dio package? Can we use them combined? if yes then how?
- How Compute works?
- How to perform multithreading? and return response so that widget can be updated?
- How do I implement a timer to execute code after a certain delay?
```dart
/// There are two ways to do that
/// 1. Timer
Timer(Duration(seconds: 2), () {
  print("Execute this code afer 2 seconds");
});
/// 2. Future:
Future.delayed(Duration(seconds: 2), () {
   print("Execute this code afer 2 seconds");
});
```

# 4. Storage

- Why SharedPreference commit method is deprecated? [Learn from here](https://stackoverflow.com/questions/57651489/sharedpreferences-commit-method-showing-deprecated-inside-flutter)
- How to persist data in Database ?

# 5. Platform Specific Android/iOS
- How does the platform channel work?
- How to perform a background job on a specific platform?
- How to send local notifications?

# 6. Dart
- Difference between these operators "?? and ?."
- Difference between Constand final? Is there any performance issue If I select one of them over another?
- What is Extention and how to use it with the existing code?
- What is typedef in Dart?
- How to handle null conditions? and use of the '??' operator.
- Use of '=>' operator?
- Differentiate between forEachand whereclause
- What is the advantage of Factory constructor?
- Why dialog inside FutureBuilder not working? [Learn from here](https://medium.com/flutter-community/flutter-threading-5c3a7b0c065f)
- Use of compareTo method? [Learn from here](https://api.flutter.dev/flutter/dart-core/num/compareTo.html)
- Advantages and Disadvantages of using static ?
- Benefits of an abstract class with a factory constructor?
  - A factory constructor allows you more control over what the constructor returns. It can return an instance of a subclass or an already existing (cached) instance.
It can return different concrete implementations based on a constructor parameter:
```dart
abstract class WidgetService {
  factory WidgetService(String type) {
    switch (type) {
      case 'a':
        return ConcreteWidgetServiceA();
      case 'b':
        return ConcreteWidgetServiceB();
      default:
        return DummyWidgetServiceA();
    }
  }
}
```
- Use of extends , interface and mixin ?
   - extends (inheritance) => Only one class can be inherited along with their public/protected members and behaviors.
   - implements (contract) => Many classes can be implemented but we have to redefine every behavior.
   - with(mixin) => Many classes can be mixed in and we can reuse the behavior of them.
   
Any class or abstract class can be used as a mixin. But if we declare mixin, it cannot be extended like a normal class or abstract class.   
```dart
class A{} //Declaring class
mixin B{} //Declaring mixin
class C extends A{} // Valid ✅
class C implements A{} // Valid ✅
class C with A{} // Valid ✅
class C extends B{} // Invalid ❌
class C implements B{} // Valid ✅
```
But a mixin cannot use another mixin.

```dart
mixin C with B{} // Invalid ❌
```
# 7. Architecture
- How to use Bloc architecture?
- How to use MVVM architecture?
- Difference between Bloc vs MVVM ?
- What is Provider state management?
- What are the different state management techniques? [Learn from here](https://flutter.dev/docs/development/data-and-backend/state-mgmt/options)

# 8. Test Cases
- How to mock objects? which classes used to do that?
- How to verify httprequest callbacks?
- How to catch the Exceptions?
- UI test cases [Learn from here](https://flutter.dev/docs/cookbook/testing/widget/introduction)


# Others
- if we change localization to the RTL language, is it changed according to language direction
- What is the use of Equatable?
- Does dart support Method Overloading?
- How we can handle the error at the project level? Is it possible to show some widgets in that case?
- How-to Encrypt and Decrypt data while making network calls?
- Difference between getDocuments() vs snapshots() in Firebase?[Learn from here](https://stackoverflow.com/questions/62610233/what-is-the-difference-between-getdocuments-and-snapshots-in-firestore/62610817#62610817)
- What is the difference between hot restart and hot reload?
- How to deal with unwanted widget build? [Learn from here](https://stackoverflow.com/questions/52249578/how-to-deal-with-unwanted-widget-build)
- What is the difference between the flutter package and the flutter plugin?
- What is the use of addPostFrameCallback ?
- How to send nested json requests to the server?
- What is the difference between 'as',' show' and 'hide' in an import statement?
- Use of export keyword?
- How to perform infinite scrolling?
- What are the ways to share images on WhatsApp, Facebook, etc?
- Difference between a Single Instance and Scoped Instance ?
- When Bad State Exception occurs? [Learn from here](https://stackoverflow.com/questions/52354195/list-firstwhere-bad-state-no-element/63300764#63300764)
- How to achieve loose coupling?
- What is a pubspec file in Dart?
- How to obfuscate Flutter apps? [Learn from here](https://medium.com/flutterworld/flutter-obfuscation-and-build-optimization-69ff5a338fdb)
- Procedure to generate release .apk(for Android) and .ipa(for iOS)
- Why a declarative UI? [Learn from here](https://flutter.dev/docs/get-started/flutter-for/declarative)



### Next questions coming soon….


### Found this project useful :heart:

* Support by clicking the :star: button on the upper right of this page. :v:

### License
```
   Copyright (C) 2020 MINDORKS NEXTGEN PRIVATE LIMITED

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
```

### Contributing to Android Interview Questions
Just make [pull request](https://github.com/jitsm555/Flutter-Interview-Questions/compare). You are in!
