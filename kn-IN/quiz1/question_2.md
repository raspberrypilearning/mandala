
--- question ---

---
legend: ಪ್ರಶ್ನೆ 2 ರಲ್ಲಿ 2
---

ನಿಮ್ಮ ಪ್ರಾಜೆಕ್ಟ್‌ನಲ್ಲಿ, ನೀವು 'My Blocks'{:class='block3myblocks'} ಇನ್‌ಪುಟ್‌ನ್ನು ಆಧರಿಸಿ ಉಡುಪುಗಳನ್ನು ಬದಲಾಯಿಸಲು ಸಂಕಲನ +ಆಪರೇಟರ್‌ ಉಪಯೋಗಿಸಿದ್ದೀರಿ.

ನಾವು ಈ ಉಡುಪುಗಳನ್ನು ಹೊಂದಿದ್ದರೆ:

![ಎಲ್ಲಾ ಉಡುಪುಗಳ ಚಿತ್ರಗಳು: ಉಡುಪು1 ಪಾರದರ್ಶಕ ದಳ; ಉಡುಪು 2 ನೇರಳೆ ದಳ; ಉಡುಪು 3 ಪಾರದರ್ಶಕ ಗೋಳ; ಮತ್ತು ಉಡುಪು 4 ನೇರಳೆ ಗೋಳ.](images/costumes_quiz.png)

ಈ ಕೆಳಗಿನ ಯಾವ ಕೋಡ್‌ ಬ್ಲಾಕ್‌ಗಳು ನಿಮ್ಮ ವಿನ್ಯಾಸವು ನೇರಳೆ ದಳದಿಂದ ನೇರಳೆ ಗೋಳವಾಗಿ ಬದಲಾಗುವಂತೆ ಮಾಡುತ್ತದೆ?

--- choices ---

- (x)

 ```blocks3
 when flag clicked
 switch costume to ((costume [number v]) + (2))
 ```

  --- feedback ---

ಹೌದು, ನೀವಿರುವ ಉಡುಪಿನ ಸಂಖ್ಯೆ ಉಡುಪು 2 ಮತ್ತು ನೀವು ಬದಲಾಗಬೇಕಾದ ಉಡುಪು, ಉಡುಪು 4, ಆದುದರಿಂದ ನೀವು ಉಡುಪು 2 + 2 = 4 ಕ್ಕೆ ಬದಲಾಗಬೇಕು.

  --- /feedback ---

- ( )
 ```blocks3
 when flag clicked switch costume to ((costume [number v]) + (1))
 ```
  --- feedback ---

ಇದು ಉಡುಪು 2 ರಿಂದ ಉಡುಪು 2 + 1 = 3 ಕ್ಕೆ ಬದಲಾಗುತ್ತದೆ. ಉಡುಪು 3 ಪಾರದರ್ಶಕ ಗೋಳ, ನೇರಳೆ ಗೋಳವಲ್ಲ.

  --- /feedback ---

- ( )
 ```blocks3
 when flag clicked switch costume to ((costume [number v]) - (1))
 ```
  --- feedback ---

ಇದು ಉಡುಪು 2 ರಿಂದ ಉಡುಪು 2 - 1 = 1 ಕ್ಕೆ ಬದಲಾಗುತ್ತದೆ. ಉಡುಪು 1 ಪಾರದರ್ಶಕ ದಳ, ನೇರಳೆ ಗೋಳವಲ್ಲ.

  --- /feedback ---

- ( )
 ```blocks3
 when flag clicked switch costume to ((1)+(1))
 ```
  --- feedback ---

ಈಗ ಯಾವ ಉಡುಪನ್ನು ತೋರಿಸಲಾಗುತ್ತಿದೆ ಅನ್ನುವುದನ್ನು ಲೆಕ್ಕಿಸದೇ ಉಡುಪನ್ನು ಇದು `costume 2`{:class='block3looks'} ಗೆ ಬದಲಾಯಿಸುತ್ತದೆ.

  --- /feedback ---

--- /choices ---

--- /question ---
