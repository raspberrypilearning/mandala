
--- question ---

---
legend: 2లో 2వ ప్రశ్న
---

మీ ప్రాజెక్ట్‌లో, మీరు 'My Blocks'{:class='block3myblocks'} ఇన్‌పుట్ ఆధారంగా costume లను మార్చడానికి అదనంగా + ఆపరేటర్‌ని ఉపయోగించారు.

మన దగ్గర ఈ costumes ఉంటే:

![అన్ని costume చిత్రాలు: costume 1 పారదర్శకమైన రేక; costume 2 ఊదారంగు రేక; costume 3 ఒక పారదర్శక భూగోళం; మరియు costume 4 పర్పుల్ గ్లోబ్.](images/costumes_quiz.png)

కింది కోడ్ బ్లాక్‌లలో ఏది పర్పుల్ రేక నుండి పర్పుల్ గ్లోబ్‌కు మారడానికి మీ నమూనాను పొందుతుంది?

--- choices ---

- (x)

 ```blocks3
 when flag clicked
 switch costume to ((costume [number v]) + (2))
 ```

  --- feedback ---

అవును, మీరు ధరించే కాస్ట్యూమ్ నంబర్ 2 మరియు మీరు మార్చాలనుకుంటున్న దుస్తులు 4 కాబట్టి మీరు కాస్ట్యూమ్ 2 + 2 = 4 కి మారాలి.

  --- /feedback ---

- ( )
 ```blocks3
 when flag clicked switch costume to ((costume [number v]) + (1))
 ```
  --- feedback ---

ఇది కాస్ట్యూమ్ 2 నుండి కాస్ట్యూమ్ 2 + 1 = 3కి మారుతుంది. కాస్ట్యూమ్ 3 అనేది పారదర్శక గ్లోబ్, పర్పుల్ గ్లోబ్ కాదు.

  --- /feedback ---

- ( )
 ```blocks3
 when flag clicked switch costume to ((costume [number v]) - (1))
 ```
  --- feedback ---

ఇది కాస్ట్యూమ్ 2 నుండి కాస్ట్యూమ్ 2 + 1 = 1కి మారుతుంది. కాస్ట్యూమ్ 1 అనేది పారదర్శక గ్లోబ్, పర్పుల్ గ్లోబ్ కాదు.

  --- /feedback ---

- ( )
 ```blocks3
 when flag clicked switch costume to ((1)+(1))
 ```
  --- feedback ---

ఇది ప్రస్తుతం ఏ costume చూపబడుతున్నా దానితో సంబంధం లేకుండా costume ను `costume 2`{:class='block3looks'}కి మారుస్తుంది.

  --- /feedback ---

--- /choices ---

--- /question ---
