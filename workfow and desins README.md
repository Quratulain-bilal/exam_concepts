Is baar maine course ka asal intro dobara parha, taake kahani ke sab hisse uske mutabiq hon. Pichle versions mein "verdict" wali line beech mein achanak aa gayi thi aur kuch hisse maine apni taraf se jode thay. Is baar line wahan hai jahan se woh naturally nikalti hai.

## Workflow kyun parhna parta hai?

**1. Kahani: do teams, ek kaam**

Do teams ne ek hi AI assistant ek hi kaam ke liye apnaya: **contract review**. Contract woh kaagaz hota hai jis mein likha hota hai ke dono parties ko kya kya karna hai, aur uski har shart ko **clause** kehte hain. Review ka matlab hai ke koi insaan parh kar dekhe ke is mein hamare liye kuch nuqsan wali baat to nahi.

**Pehli team** ne kaam ko step by step map kiya. AI ne clauses nikale, company ke apne rules (playbook) se hatne wali baatein flag kiye, aur **redline** likha. Redline contract ka woh marked-up version hota hai jis mein dikhta hai ke hum kya badalna chahte hain. Phir **har change ko ek lawyer ne approve kiya.** Natija: review ka waqt takreeban aadha ho gaya aur quality bhi barqarar rahi.

**Doosri team** ne poora process AI ke saamne rakh diya. AI ne draft achha likha, to team ne socha ke chhote risk wale clauses ka approval bhi isi ko de dein, **bina kisi insaan ke dekhe.** Ek mahine ke andar ek approved clause ne aisi zimmedari bana di jo kisi ne pakri nahi, aur team ne tool poora hata diya.

**2. Ab sawal**

Product wohi, process wohi, model wohi. Phir ek team kamyab aur doosri nakam kyun hui? Course ka jawab: **farq sirf is mein tha ke har team ne kaunse steps AI ko diye.**

**3. Ab ek chhoti ghalti jo aap ke saath bhi hui hogi**

Aap ne AI se kuch manga aur jawab disappointing aaya. Phir aap ne ya to keh diya "yeh tool yeh kar hi nahi sakta", ya lafz badalti rahin jab tak kuch kaam na kar gaya. Yeh pehli kahani se ulta lagta hai, lekin course kehta hai ke yeh **wohi ek ghalti hai, do taraf se**:

```
Doosri team: achha draft dekha  --> samjha "step safe hai, AI ko de do"
Aap:         bura output dekha  --> samjha "task impossible hai"
```

Dono ne **output ko faisla** bana liya.

**4. Isi se woh line nikalti hai**

> **"The output is not the verdict."**

**Verdict** ka matlab hai final faisla, jaise court ka. Output sirf ek nateeja hai, faisla nahi. Achha output dekh kar yeh faisla nahi hota ke step AI ko dena theek hai, aur bura output dekh kar yeh faisla nahi hota ke task ho hi nahi sakta. Faisla **step ke baare mein** hota hai, aur uske sawal hum aage seekhenge: kya yeh step undo ho sakta hai, ghalti ka nuqsan kitna hai, aur jawabdeh kaun hai.

**5. Is liye design**

Agar faisla output se nahi hota, to usay **pehle se, soch kar** tay karna parega. Isi ko hum workflow design kehte hain.

## Concept 1: Step, aur do aadatein

Ab dekhte hain ke "AI use karna" ke do bilkul alag matlab hote hain.

**Pehla: "I use AI."** Yeh ek **personal habit** hai. Yeh aap ke dimagh mein rehti hai, aap ke **mood** ke saath badalti hai, aur jab aap **chutti** par hon to ghayab ho jati hai.

**Doosra: "Our workflow uses AI."** Yeh ek **repeatable process** hai jo ek team chalati hai, jahan AI named steps har baar same tarah karta hai, chahe keyboard par koi bhi ho.

Course kehta hai ke **sirf doosri cheez ki value barhti hai, aur sirf doosri cheez aisi ghalat ho sakti hai jo baar baar ghalat hoti rahe.** Is liye usay design karna zaroori hai.

**Step kya hai?**

> **Step = workflow ka ek named hissa, jis ka ek owner ho.**

Aur ek aur farq jo yaad rakhein:

```
Session  --> aap baad mein judge karti hain: "mujhe result pasand aaya?"
Step     --> aap pehle se tay karti hain, aisi wajahon par jo is baat
             se nahi badalti ke aaj output achha dikha ya nahi
```

Yehi baat "output is not the verdict" ki dobara hai: step ka faisla output dekh kar nahi, pehle se hota hai.

## Ek nazar mein poora flow

```
Do teams, same AI, same kaam
        |
        v
Ek ne steps tay kiye (kamyab), ek ne sab de diya (nakam)
        |
        v
Sawal: farq kahan tha?  --> kaunsa step kis ko diya gaya
        |
        v
Aam ghalti bhi wohi: output ko faisla bana lena
        |
        v
"The output is not the verdict"
        |
        v
Isi liye pehle se design: steps, har step ka ek owner
        |
        v
"I use AI" (habit) vs "our workflow uses AI" (process)
```
##Concept 2 se link

Concept 1 mein humne seekha ke har step ka owner pehle se tay hota hai. Lekin owner tay karne se pehle ek sawal aata hai: kaam hai kya? Agar kaam hi saaf nahi, to uske steps aur owners tay karna bekaar hai. Isi liye workflow design ka pehla kaam yeh hai: messy cheez ko saaf requirements mein badalna.
## Concept 2, 

**Masla:** aap ko kaam aksar saaf nahi milta. Kabhi 40 page ka lamba document, kabhi adhoore emails, kabhi sirf ek jumla jaise "hamein better reporting chahiye".

Is par AI se kaam shuru karwa dein to woh khali jagahein khud bhar dega, aur jawab sahi dikhega magar aap ka maqsad nahi hoga. Isi liye pehle kaam ko saaf karte hain.

## Teen kaam, ek ke baad ek

**1. Kaam ko saaf likho.**
Agar sirf ek jumla mila ho to 5 sawalon ke jawab likho:

```
Kya banega?  Kis ke liye?  Kitni baar?  Kis data se?  Kis format mein?
```

Misaal: "Har Monday subah manager ke liye, sales data se, ek PDF report."

Agar documents mile hon to AI se kaho: "Is se saari requirements ki table banao, aur har ek ke saath likho ke document ke kis hisse se aayi." **Requirement** matlab woh cheez jo kaam mein hamein chahiye.

**2. Jo jawab nahi mila, wahan AI ko mat bharne do.**
Us jagah ek sawal poochho: "Kitne din mein chahiye?" AI se kaho: "Jo maine nahi bataya, wahan bolo ke nahi bataya." Warna AI andaza laga kar bhar dega.

**3. Phir apni hi list mein ghalti dhoondo (isay course attack kehta hai).**
AI se poochho: kaunsi requirement ambiguous hai (do matlab nikal sakte hain)? Kaunsi ko do log alag samjhenge? Kaunsi baat likhi nahi magar zaroori hai?

## Ek example, teeno saath

Requirement mili: **"Report promptly deliver ho."**

```
Attack: "promptly" kya hai? Kisi ke liye 2 din, kisi ke liye 2 hafte.
        Do teams do alag process bana lengi.
Sawal:  "Month end ke kitne din ke andar chahiye?"
Jawab:  "2 din."
Naya:   "Report month end ke 2 din ke andar deliver ho."
```

Ab isay **check** kar sakte hain: 2 din mein aayi ya nahi. Course ka test yehi hai: **agar aap uska check nahi likh sakti, to woh requirement abhi decide hi nahi hui.**

## Yeh sab kyun?

```
Ghalti shuru mein pakri   --> 1 sawal poochha, kaam khatam
Ghalti baad mein pakri    --> poora kaam dobara
```

## Ek line mein

> Kaam shuru karne se pehle use saaf likho (5 sawal ya requirements ki table), jo missing ho woh poochho, aur phir har requirement mein dhoondo ke koi ambiguous to nahi.


## Concept 3: Jo number matter karta hai, usay compute karo, likho mat

**Concept 2 se link:** ab kaam saaf ho gaya (requirements, 5 sawal). Lekin planning ke kaam mein **numbers** aate hain, jaise "kitne analysts chahiye?". Yahan ek nayi baat samajhni hai.

## Planning mein do alag kaam hote hain

```
Synthesis    = kai cheezein jama karke OPTIONS banana
               (AI yeh achha karta hai, kai factors ek saath sambhalta hai)

Calculation  = numbers nikalna
               (yahan khatra hai)
```

## Calculation mein khatra kya hai?

Aisa nahi ke AI jama tafreeq nahi kar sakta, woh kar sakta hai. Masla yeh hai:

> **Page par dekh kar pata nahi chalta ke number calculate hua ya sirf likha gaya.** Dono ek jaise dikhte hain.

```
Likha hua number:      "Growth 14% hai"
Calculate hua number:  "Growth 14% hai"

Dono sahi lagte hain. Ek ghalat ho to nazar nahi aata.
```

## Is liye ek rule

> **Agar result matter karta hai, to compute karo. Kabhi likhwao mat.**

Ghar ka example (meri apni misaal): dukandar zubani bol de "total 2,340 hua", ya calculator par jor kar dikhaye. Dono ka jawab ek jaisa dikhta hai, lekin calculator wale ko aap dobara check kar sakti hain.

## "Compute" kaise karwate hain? Code execution

**Code execution** = AI ek chhota sa code likhta hai, chalata hai, aur jo nikla woh report karta hai.

Course ka example: staffing plan.

```
Andaze (guess) par bana plan   --> "table mein ek guess"
Asli timesheet data par bana   --> har number tak line by line pahunch sakte hain,
                                   koi bhi dobara chala kar check kar sakta hai
```

Prompt ka tareeqa (course se): pehle **computation**, phir **recommendation**, aur assumptions bhi maango:

```
"Ticket data par code execution se quarterly volume growth aur
 average tickets per analyst calculate karo. Phir un figures se
 headcount recommend karo aur assumptions dikhao."
```

Assumptions is liye maange ke koi aap ki recommendation se ittefaq na kare to poora hisaab dobara na karna paray.

## Ek limit

Code chalta exact hai, lekin **code AI ne likha hai**, aur woh ghalat column utha sakta hai. Is liye dekho ke **kya compute hua**, sirf yeh nahi ke compute hua.

## Ek diagnostic habit

Agar numbers thode ghalat aa rahe hain, to aksar wajah prompt nahi hoti. Wajah yeh hoti hai ke calculation **text mein** maangi gayi thi.

## Viva ke liye ek line

> Planning mein synthesis (options banana) AI achha karta hai, lekin jo number matter karta hai usay code execution se compute karte hain, likhwate nahi, kyunke likha aur calculate hua number page par ek jaisa dikhta hai, aur compute hone ke baad bhi check karte hain ke code ne kya use kiya.
Concept 4: Window test

Concept 3 se link: options banana (synthesis) AI ka achha kaam hai, magar AI sirf wohi dekh sakta hai jo aap usay dete hain. Sawal yeh hai: kaunse steps AI ko dein?

Kahani (course ki): ek operations lead ne AI se poora capacity plan manga, aur AI ne likha “3 analysts hire karo.” Plan achha structured tha. Lekin team par do hafte pehle hiring freeze (hiring band) lag chuka tha, jo meeting mein announce hua tha, kisi file mein nahi. AI ko pata hi nahi tha.

Ghalti data ki nahi thi. Ek step ko aisi cheez chahiye thi jo AI tak pahunch hi nahi sakti thi.

Do qisam ke steps
Synthesis step   Inputs aap supply kar sakti hain  --> AI ko de sakte hain
Judgment step    Inputs aap supply nahi kar sakti  --> insaan ka
                 (hiring freeze, risk appetite)

Judgment insaan ka isliye nahi ke judgment koi muqaddas cheez hai. Is liye ke uske inputs available hi nahi.

AI ruk kar nahi kehta

Input missing ho to AI ruk kar nahi kehta “mujhe pata nahi.” Woh khali jagah ko “aise faisle aam taur par kaise hote hain” se bhar deta hai, aur utne hi confidence se jitna asal calculate kiye hue hisse mein tha. Isi liye ghalti nazar nahi aati.

## Concept 4: Window test (polished version)

Concept 3 mein humne dekha ke AI options banane (synthesis) mein achha hai. Ab sawal yeh hai ke **kaunsa step AI ko dein?** Is ka pehla test **window test** hai.

**Window** woh sab hai jo model is kaam ke liye dekh sakta hai: aap ka prompt, aap ki files, aur ab tak ki baat cheet. AI sirf wohi jaanta hai jo window ke andar hai.

**Test har step par lagta hai, poore kaam par nahi.** Har step ke liye poochein:

> **Kya is step ki saari zaroori info main likh kar AI ke saamne rakh sakti hun?**

```
HAAN  --> Step AI ke liye eligible hai.
          AI us info par achhi synthesis kar ke options bana sakta hai.

NAHI  --> Yeh judgment step hai, aur insaan ka rehta hai.
```

**Nahi wale step insaan ka kyun rehte hain?** Kyunke jo info window mein nahi, AI ko woh milti hi nahi. Lekin AI ruk kar nahi kehta "mujhe pata nahi." Woh khali jagah ko "aise faisle aam taur par kaise hote hain" se bhar deta hai. Koi error nahi aata, jawab confident dikhta hai, lekin aap ki asli situation ke mutabiq nahi hota.

**Kahani (course ki):** AI ne capacity plan mein "3 analysts hire karo" likha, jabke team par hiring freeze tha, jo meeting mein hua tha aur kisi file mein nahi. Ghalti data ki nahi thi. Ek step ko aisi info chahiye thi jo AI tak pahunch hi nahi sakti thi.

```
Capacity plan ke steps:
  Trend aur options nikalna  --> info window mein hai   --> AI ko de sakte hain
  Hiring ka final faisla     --> info window ke bahar   --> insaan ka
```

Yani ek hi kaam ke andar kuch steps AI ko jate hain aur kuch insaan ke paas rehte hain.

**Do baatein jo zaroor yaad rakhein:**

1. **Pass hone ka matlab yeh nahi ke step AI ko mil gaya.** Window test sirf yeh batata hai ke step **eligible** hai. Uske baad step ko Part 2 ke **teen criteria** (reversibility, stakes, accountability) se bhi guzarna hai.
2. **Judgment insaan ka isliye hai ke inputs available nahi, is liye nahi ke judgment koi muqaddas cheez hai.** Agar woh info likh kar di ja sakti ho ("hamare yahan hiring freeze hai"), to woh window mein aa jati hai.

**Research par bhi lagta hai:** model ka knowledge ek tareekh par ruk jata hai, aur uske baad ki cheez window ke bahar hai. Stable concept ke liye model ka knowledge theek hai, lekin current, price ya date wali cheez ke liye external source maango jo aap khol sakein, link ke saath.

### Viva ke liye ek line

> Window test mein har step par poochte hain ke uski saari zaroori info model ke saamne rakhi ja sakti hai ya nahi. Haan to step AI ke liye eligible hai (phir teen criteria), nahi to woh judgment step hai aur insaan ka rehta hai, kyunke AI missing info ko confident andaze se bharta hai.

**Part 1 (Design) mein humne yeh seekha:** pehle yeh samjha ke "I use AI" ek personal habit hai jabke workflow named steps ka repeatable process hai jahan har step ka ek owner hota hai, aur course ki buniyadi baat yeh ke "the output is not the verdict", yani achha ya bura output dekh kar faisla nahi hota. Phir seekha ke kaam shuru karne se pehle use saaf karte hain: messy documents se requirements ki table (source ke saath) ya ek jumle se 5 sawalon ke jawab (kya banega, kis ke liye, kitni baar, kis data se, kis format mein) nikalte hain, jo jawab missing ho woh AI se nahi bharwate balkay clarifying question poochte hain, aur phir har requirement par attack karte hain ke ambiguous ya implied to nahi. Phir yeh ke jo number matter karta hai usay code execution se compute karte hain, likhwate nahi. Aakhir mein window test: step ki saari info AI ko likh kar di ja sakti ho to step eligible hai (synthesis, yani options banana), aur nahi di ja sakti to woh judgment step hai jo insaan ka rehta hai, kyunke AI missing info ko confident andaze se bhar deta hai. **Ab Part 2 (Delegation Map) mein hum seekhenge** ke jo steps window test se guzar gaye, un ka owner kaise tay karein: har step par teen criteria (reversibility, stakes, accountability) lagte hain aur natija AI, Collaborative ya Human nikalta hai, phir dekhenge ke do alag workflows mein same pattern kyun aata hai, map kin teen tareeqon se ghalat hota hai (halo delegation, unstaffed gate, tool ko map karna), aur map ko sach rakhne ke liye ek named map owner aur quarterly review kyun chahiye.

## Part 2 shuru: Concept 5, teen criteria

**Part 1 se link:** Part 1 mein kaam saaf hua aur window test se pata chala ke kaunsa step AI ke liye eligible hai. Lekin eligible hone ka matlab yeh nahi ke AI ko mil gaya. Ab sawal yeh hai: **har step ka owner kaun hoga?** Course har step par teen alag faisle karta hai: (1) **Eligibility**: kya AI is ko chhu bhi sakta hai? (window test yahin tha), (2) **Ownership**: owner kaun? (yeh concept), (3) **Implementation**: kaun sa tool usay chalayega? Teeno ko mix karne se aisa map banta hai jo theek lagta hai magar ghalat hota hai.

## Pehle: teen possible owner

Pehle workflow ke steps ko order mein likho, phir har step ko in teen mein se ek mein daalo:

```
AI-appropriate   AI is step ka owner ho sakta hai
Human-retained   insaan is step ka pura owner hai
Collaborative    AI banata hai, ek named insaan judge karta hai
```

## Phir: teen criteria (sirf yehi teen)

Yeh teeno sawal **step ke baare mein** hain, model ke baare mein nahi.

```
1. Reversibility   Agar AI ghalat kare to kya undo ho sakta hai?
                   Draft dobara likh sakte hain; bheji hui email wapas nahi aati.

2. Stakes          Bad case mein ghalti ki cost kya hai? (average mein nahi)
                   Galat label = 1 minute. Galat penalty figure = jitni penalty hai.

3. Accountability  Kya yeh step khud wo faisla hai jis ka insaan jawabdeh hai,
                   ya sirf ek input hai jise woh aage judge karega?
```

**Accountability ko aasan samjhein:** har step ka koi na koi jawabdeh hota hi hai, to sirf "jawabdeh kaun?" poochne se har step insaan ka ban jata. Asal sawal yeh hai ke **step khud faisla hai ya sirf input.** Agar step khud faisla hai, to uske baad kuch nahi bachta jo usay sambhale, is liye woh insaan ka. Agar step ek input banata hai jise insaan aage judge karta hai, to AI ko diya ja sakta hai, kyunke jawabdehi judge karne par hai. Dono surat mein **jawabdehi kabhi machine par nahi jati**, kyunke machine se poochha nahi ja sakta.

## Teen zaroori baatein

**1. Yeh score nahi, teen sawal hain.** Aap jama nahi kar rahi aur teen "haan" ka intezar nahi. Aksar ek criterion step decide karta hai aur baaqi do us se agree karte hain. Us ek ka naam likho taake koi aur check kar sake.

**2. Jahan jawab alag aayein, wahan sab se strict jeetta hai.** Step undo ho sakta ho aur sasta ho, lekin agar woh khud wo faisla hai jis ka insaan jawabdeh hai, to step insaan ka rehta hai.

**3. "Is step mein AI ne test run mein kitna achha kaam kiya" criterion nahi hai.** Yeh kyun, Concept 7 mein aayega (wohi Team 2 wali ghalti).

## Course ka example

```
Sign aur send karna       --> Human   (reversibility ne decide kiya: bheja hua wapas nahi aata)
Har change approve karna  --> Human   (accountability ne decide kiya: yeh khud faisla hai)
```

## Viva ke liye ek line

> Har step par teen sawal lagte hain: reversibility (undo ho sakta hai?), stakes (bad case mein cost?) aur accountability (kya yeh step khud wo faisla hai jis ka insaan jawabdeh hai?). Jawab alag aayein to sab se strict jeetta hai, aur natija AI-appropriate, Collaborative ya Human-retained hota hai.
## Concept 6: Do workflows, same criteria, alag jawab

**Concept 5 se link:** Concept 5 mein teen criteria seekhe. Ab sawal yeh hai ke kya yeh criteria sach mein kaam karte hain? Course do bilkul alag workflows par wohi criteria lagata hai aur dikhata hai ke pattern dono mein ek hi nikalta hai.

### Workflow 1: Contract review

| Step | Owner | Kis criterion ne decide kiya | Carried by |
|---|---|---|---|
| Contract se clauses nikalna | AI | Reversible, low stakes | Skill |
| Playbook se departures flag karna | AI | Reversible, ghalti redline par pakri jati hai | Skill |
| Redline aur rationale draft karna | Collaborative | High stakes, is liye insaan har edit judge karta hai | Skill + gate |
| Penalty clause ka financial exposure compute karna | AI | Reversible, aur agle gate par check hota hai | Code execution |
| Har change approve ya reject karna | Human | Yeh step khud wo faisla hai jis ka insaan jawabdeh hai | Named reviewer |
| Sign aur send karna | Human | Irreversible aur externally binding | Named signer |

Is table mein do rows par log ghalti karte hain.

**1. Penalty-exposure wali row.** Arithmetic hone ka matlab low-stakes hona nahi hai. Yeh figure approval ke faisle mein jati hai, aur figure ghalat to approval ghalat. Yeh step AI ko is liye diya ja sakta hai ke:
- result undo ho sakta hai, aur
- agli row mein insaan ke saamne aa jata hai.

Agar woh gate hata dein to step AI-appropriate nahi rehta, jabke arithmetic wohi hai. Isi liye "compute karna zaroori hai" **Carried by** column mein jata hai, **Criterion** column mein kabhi nahi. (Yeh Concept 5 wali "teen alag faisle" ki baat hai: ownership aur implementation ko mix na karein.)

**2. Playbook wali row.** Is workflow mein flag karna AI ko is liye mila ke agle row par koi flags parhta hai, aur ghalat flag ghalat redline ban kar dikh jata hai. Yehi step aise workflow mein jahan flags ke baad koi nahi parhta (jaise travel policy se expenses check karna), **Collaborative** ban jata hai.

> Step wohi raha. Farq is se parta hai ke us ke baad koi khara hai ya nahi.

Dhyan dein, AI beech mein asli kaam kar raha hai, redline ka draft bhi, jo asli legal writing hai. Insaan ke paas faisle aur woh actions hain jo undo nahi hote. Baaqi sab AI ke paas gaya.

### Workflow 2: Onboarding documents (bilkul alag field)

| Step | Owner | Kis criterion ne decide kiya | Carried by |
|---|---|---|---|
| HR system export se new-hire details nikalna | AI | Reversible, confirmation step par check hota hai | Code execution |
| Approved template se offer letter draft karna | AI | Reversible draft, bhejne tak low stakes | Skill |
| Welcome note personalise karna | Collaborative | Manager ki awaaz window mein nahi aa sakti | Named reviewer |
| Compensation approved req se match karna confirm karna | Human | Yeh step khud check hai, is ke baad kuch nahi | Named reviewer |
| Signed offer bhejna | Human | Irreversible aur externally binding | Named signer |

### Pattern jo dono mein aaya

- **Mechanical aur draft steps** AI ko gaye, dono maps mein.
- **Figure confirm karne wala step** aur **jo step undo nahi hota**, dono mein insaan ke paas rahe.
- Yeh kisi ke zauq ne decide nahi kiya. **Criteria ne do alag fields mein do baar decide kiya.**

Is se yeh bhi nikalta hai ke map banate waqt "AI is field mein achha hai ya nahi" poochne ki zaroorat nahi, sirf step par teen sawal lagane hain.

### Yaad rakhne wali baatein

1. "Compute karna zaroori hai" implementation hai, criterion nahi. Isko reason bana kar high-stakes calculation bina review ke AI ko dena ghalti hai.
2. Ek step ki safety is par depend karti hai ke us ke **baad kya hai**, sirf us step par nahi.
3. Gate hatao to step ka owner badal jata hai, chahe step ka kaam wohi rahe.

### Viva ke liye ek line

Contract review aur onboarding bilkul alag kaam hain, magar wohi teen criteria lagane se pattern same aaya: mechanical aur draft steps AI ko, aur figure confirm karne wala ya irreversible step insaan ko. "Computed hona chahiye" Carried-by column ki baat hai, criterion ki nahi, aur ek step ki safety is par hai ke us ke baad koi jaanchne wala khara hai ya nahi.



