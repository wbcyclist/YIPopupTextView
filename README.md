YIPopupTextView
===============

facebook's post-like input text view for iOS.

<img src="https://github.com/downloads/inamiy/YIPopupTextView/screenshot.png" alt="ScreenShot1" width="225px" style="width:225px;" />

How to use
----------
```
// NOTE: maxCount = 0 to hide count
YIPopupTextView* popupTextView = [[YIPopupTextView alloc] initWithPlaceHolder:@"input here" maxCount:1000];
popupTextView.delegate = self;
popupTextView.showCloseButton = YES;
popupTextView.caretShiftGestureEnabled = YES;   // default = NO
popupTextView.text = self.textView.text;
//popupTextView.editable = NO;                  // set editable=NO to show without keyboard
[popupTextView showInView:self.view];

//
// NOTE:
// You can add your custom-button after calling -showInView:
// (it's better to add on either superview or superview.superview)
// https://github.com/inamiy/YIPopupTextView/issues/3
//
// [popupTextView.superview addSubview:customButton];
//

```

For `caret-shifting`, it is better to use [YISwipeShiftCaret](https://github.com/inamiy/YISwipeShiftCaret) for all UITextField/UITextViews.


License
-------
YIPopupTextView is available under the [Beerware](http://en.wikipedia.org/wiki/Beerware) license.