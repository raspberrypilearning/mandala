
--- question ---

---
legend: 2 में से दूसरा प्रश्न
---

अपने प्रोजेक्ट में, आपने 'My Blocks'{:class='block3myblocks'} इनपुट के आधार पर पोशाक बदलने के लिए जोड़ + ऑपरेटर का इस्तेमाल किया।

अगर हमारे पास ये पोशाकें हैं:

![सभी परिधानों की छवियां: पोशाक 1 एक पारदर्शी पंखुड़ी है; पोशाक 2 एक बैंगनी पंखुड़ी है; पोशाक 3 एक पारदर्शी ग्लोब है; और पोशाक 4 एक बैंगनी ग्लोब है।](images/costumes_quiz.png)

निम्नलिखित में से कौन सा कोड ब्लॉक बैंगनी पंखुड़ी से बैंगनी ग्लोब पर स्विच करने के लिए आपका पैटर्न प्राप्त करेगा?

--- choices ---

- (x)

 ```blocks3
 when flag clicked
 switch costume to ((costume [number v]) + (2))
 ```

  --- feedback ---

हां, आप जिस पोशाक नंबर पर हैं, वह पोशाक 2 है और आप जिस पोशाक पर स्विच करना चाहते हैं, वह पोशाक 4 है, इसलिए आपको पोशाक 2 + 2 = 4 पर स्विच करना होगा।

  --- /feedback ---

- ( )


 ```blocks3
 when flag clicked 
 switch costume to ((costume [number v]) + (1))
 ```

  --- feedback ---

This will switch from costume 2 to costume 2 + 1 = 3. Costume 3 is the transparent globe, not the purple globe.

  --- /feedback ---

- ( )


 ```blocks3
 when flag clicked 
 switch costume to ((costume [number v]) - (1))
 ```

  --- feedback ---

This will switch from costume 2 to costume 2 - 1 = 1. Costume 1 is the transparent petal, not the purple globe.

  --- /feedback ---

- ( )

 ```blocks3
 when flag clicked 
 switch costume to ((1)+(1))
 ```

  --- feedback ---

यह पोशाक को `costume 2`{:class='block3looks'} में बदल देगा, भले ही वर्तमान में कोई भी पोशाक दिखाई जा रही हो।

  --- /feedback ---

--- /choices ---

--- /question ---
