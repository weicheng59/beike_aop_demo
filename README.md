# beike_aop_demo
 
flutter pub get
flutter run --release --no-sound-null-safety

click the add button and following error will show in console
also the click is not working and whole app go unresponsive

I/flutter (22167): type '_OneByteString' is not a subtype of type 'int' of 'index'
I/flutter (22167): #0      PointCut.aop_stub_47 (package:beike_aspectd/src/plugins/aop/annotation/pointcut.dart)
I/flutter (22167): #1      PointCut.proceed (package:beike_aspectd/src/plugins/aop/annotation/pointcut.dart)
I/flutter (22167): #2      ClickAopHook.hookInvokeCallback (package:beike_aop_demo/hook_entry_points.dart:34)
I/flutter (22167): #3      new _GrowableList._literal2 (dart:core-patch/growable_array.dart)
I/flutter (22167): #4      TapGestureRecognizer.handleTapDown (package:flutter/src/gestures/tap.dart)
I/flutter (22167): #5      BaseTapGestureRecognizer._checkDown (package:flutter/src/gestures/tap.dart:289)
I/flutter (22167): #6      BaseTapGestureRecognizer.acceptGesture (package:flutter/src/gestures/tap.dart:267)
I/flutter (22167): #7      GestureArenaManager.sweep (package:flutter/src/gestures/arena.dart:157)
I/flutter (22167): #8      GestureBinding.handleEvent (package:flutter/src/gestures/binding.dart:449)
I/flutter (22167): #9      GestureBinding.dispatchEvent_aop_stub_58 (package:flutter/src/gestures/binding.dart:425)
I/flutter (22167): #10     PointCut.aop_stub_58 (package:beike_aspectd/src/plugins/aop/annotation/pointcut.dart)
I/flutter (22167): #11     PointCut.proceed (package:beike_aspectd/src/plugins/aop/annotation/pointcut.dart)
I/flutter (22167): #12     ClickAopHook.hookHitTest (package:beike_aop_demo/hook_entry_points.dart:27)
I/flutter (22167): #13     new _GrowableList._literal2 (dart:core-patch/growable_array.dart)

it was tested on android only

