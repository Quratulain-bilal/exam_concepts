
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


## Concept 7: Map ghalat hone ke teen tareeqe

**Concept 6 se link:** Concept 6 mein dekha ke criteria lagane se sahi map banta hai. Ab dekhte hain ke map **ghalat kaise** banta hai. Yeh Concept 5 wale "AI ne test run mein kitna achha kiya criterion nahi hai" ka jawab bhi hai.

### Kahani: Team 2 ki ghalti

Team 2 koi laparwah team nahi thi. Unhon ne hafton dekha ke AI redline achhi draft karta hai, phir kaha "chalo asaan clauses approve bhi yehi kar le." Yeh evidence par mabni, samajhdar lagne wala faisla tha, aur isi tarah risk chupke se workflow mein ghus jata hai.

**Over-delegation** ka matlab hai AI ko step ke risk se zyada de dena. Yeh "inaam" ki wajah se hota hai: draft achha aata raha, to agla step bhi safe lagne laga. Magar agla step ek **alag qism ka step** hai.

> **Draft ka achha hona draft ke baare mein evidence hai, faisle ke baare mein nahi.**

Over-delegation teen shaklon mein aati hai, aur teeno ke reasons sach hote hain.

### 1. Halo delegation

**Matlab:** Pichla step achha gaya, is liye agla step bhi AI ko de dena.

Misaal: AI complaints ki summary achhi banata hai. Is liye aap severity (low, medium, high) bhi usi ko de deti hain. Magar severity decide karti hai ke customer ko escalate karna hai ya nazar-andaz karna. High complaint miss ho gayi to hafte baad dobara classify karne se bhi ghalti theek nahi hoti. Summary ki quality ek step ki kaabiliyat thi, severity doosra step hai.

### 2. Unstaffed gate

**Matlab:** Collaborative step jahan review ab asal mein ho nahi raha.

Shuru mein reviewer dhyan se parhta hai. Phir queue lambi ho jati hai, ya drafts do mahine se achhe aa rahe hain, to review ek nazar bana, phir sirf click. Kisi ne map nahi badla, magar step ab **automated ho chuka hai**. Map yeh nahi batata, kyunke map wohi dikhata hai jo aap ne design kiya tha, jo chal raha hai woh nahi.

Is ka test: "Pichle hafte kis ne review kiya, aur kitni der?" Agar koi jawab nahi de sakta, to gate khali hai.

### 3. Tool ko map karna, kaam ko nahi

**Matlab:** Team ek achha feature banati hai aur workflow us feature ki shakal ka ban jata hai.

Misaal: "Hamara summarising Skill bohat achha hai, to workflow mein ek summary step daal dete hain." Wajah yeh nahi ke kaam ko summary chahiye, wajah yeh hai ke Skill achha hai. Isay andar se dekhna sab se mushkil hai, kyunke tool waqai achha chal raha hota hai, bas woh kaam nahi hota.

### Course ka complaint workflow (teeno ghaltiyan ek saath)

| Step | Owner | Di gayi wajah |
|---|---|---|
| Complaint aur ticket history nikalna | AI | Mechanical retrieval |
| Complaint ko issue template mein summarise karna | AI | Hamara Skill is mein bohat achha hai |
| Severity classify karna | AI | Teen mahine se summaries sahi aa rahi hain |
| Customer ka jawab draft karna | Collaborative | AI draft kare, duty agent bhejne se pehle dekhe |
| Jawab bhejna | AI | Sirf low severity, aur drafts strong hain |
| CRM mein outcome likhna | AI | Mechanical write |

**Diagnosis:**

- **Row 3 halo delegation hai.** Wajah "summaries sahi hain" di gayi, jabke severity alag step hai aur us ke baad koi call dobara nahi parhta. Zyada se zyada collaborative hona chahiye.
- **Row 5 over-delegation hai** (aur row 4 se aayi hai). "Sirf low severity" control lagta hai, magar severity row 3 mein usi system ne set ki jo ab bina review ke bhej raha hai. Step apne aap ko gate skip karne ki ijazat nahi de sakta. Aur bhejna undo bhi nahi hota.
- **Row 2 tool ko map karna hai.** Wajah "Skill achha hai" hai, "kaam ko aisa chahiye" nahi.
- **Row 4 theek hai, magar nazar rakhein.** Duty agent har draft dekhta hai, magar kisi ne nahi kaha ke ek shift mein kitne drafts hote hain. Gate sahi design hai, magar uske peeche capacity check nahi.

Dhyan dein, har di gayi wajah **sach thi**. Skill waqai achha hai, summaries waqai sahi thi. Ghalat map ghalat step ke baare mein sach baaton se bantay hain.

### Check karne ka tareeqa (is order mein)

1. Pehle kaam ko bina kisi tool ke map karein.
2. Har step ko alag alag classify karein.
3. Har collaborative step par poochein: **kaun review kar raha hai, aur kab?** Gate abhi tak staffed hain ya nahi, yeh aap ko regularly poochna hai.

### Viva ke liye ek line

Map teen tareeqon se ghalat hota hai: halo delegation (pichla step achha gaya to agla de diya), unstaffed gate (review sirf click ban gaya aur step chupke se automate ho gaya), aur tool ko map karna (feature ke hisaab se workflow bana, kaam ke hisaab se nahi). In sab ki wajah yeh hai ke "drafting achi hai" draft ka evidence hai, faisle ka nahi.

## Concept 8 

**Masla:** Map ek baar likha jata hai, phir workflow badalta rehta hai (naya step, naya reviewer, zyada kaam), magar map wahin purana rehta hai. Aur koi alarm nahi bajta.

**Misaal:** Aap ne dukaan ka register banaya ke "Ali roz stock check karega." Teen mahine baad Ali chala gaya, ya kaam double ho gaya, magar register mein ab bhi wohi likha hai. Sab samajhte hain stock check ho raha hai, jabke nahi ho raha.

**Hal (sirf do cheezein):**
1. **Ek named owner:** ek insaan jo dekhe ke map ab bhi sach hai. Team nahi, kyunke "koi aur dekh lega" wali soch se kisi ke paas zimmedari nahi rehti.
2. **Review ki tareekh:** har 3 mahine baad map dobara parhein.

**Review mein sab se zaroori sawal:** "Pichle hafte is step ko kis ne check kiya, aur kitni der?" Agar koi nahi bata sakta, to woh step asal mein automate ho chuka hai.

**Viva ke liye ek line:** Map dheere dheere ghalat hota hai aur koi alarm nahi bajta, is liye ek named owner aur quarterly review chahiye.

Clear hai to "next" likhein, Part 3 (Concept 9) shuru karte hain.

## Concept 9: Build loop (ideate, prototype, feedback, refine)

**Part 2 se link:** Part 2 mein tay hua ke kaun sa step kis ka hai. Ab Part 3 mein dekhte hain ke AI ke saath cheez **banate** kaise hain.

### Main baat

AI ek vending machine nahi, **design partner** hai. Aap "solution de do" keh kar solution nahi lete. Aap ek loop chalate hain, 4 steps ka:

1. **Ideate:** options banwana
2. **Prototype:** ek option ko itna concrete banana ke us par react kar sakein
3. **Feedback:** dekhna ke kya ghalat hai (jo pehle se pata nahi hota)
4. **Refine:** woh theek karna, phir dobara loop

Loop ek **Project** ke andar chalayein, taake background, limits aur pichle faislay stable rahein. Alag alag chats mein har round naye sire se shuru hota hai, aur aap ke paas drafts ka dher bantay hai, solution nahi.

### Course ka example: dashboard (3 cycles)

Ek analytics team ko 5 metrics track karne ka chhota tool chahiye tha. Unhon ne AI se ek **artifact** (chat ke andar bana chhota working web page) banwaya.

| Cycle | Kya maanga | Kya hua |
|---|---|---|
| 1 | 5 metrics ka dashboard, har ek ka chart | Kaam kar gaya. Is cycle se log overconfident ho jate hain |
| 2 | Date filter aur totals row | Filter chala, **totals ghalat**. Dekhne mein sahi lagte the, ek analyst ne pakra kyunke usay andaza tha |
| 3 | Brand colors aur print layout | Pehli baar mein theek |

**Cycle 2 mein kya hua?** Totals **likhe gaye the, compute nahi hue the**. Yeh Concept 3 hai: jo number matter karta hai, usay code execution se compute karo.

### Sab se zaroori sabaq

- **Cycle 3 description ka masla tha:** behtar batane se hal ho gaya.
- **Cycle 2 feature ka masla tha:** kitna bhi behtar describe karo, hal nahi hota. Hal yeh tha ke calculation code execution mein jaye.

> In dono ko alag pehchanna hi asal skill hai. Part 4 is ka tareeqa batata hai.

### Cycle 2 beech mein kyun?

Kyunke asli khatarnak ghalti **khamoshi se** aati hai. Loud error (error message) kuch nahi sikhata, woh bata deta hai kahan dekhna hai. Asal khatra woh hai jo review se guzar jaye, kyunke output smooth, formatted aur confident tha.

### Viva ke liye ek line

AI ke saath build karna ek loop hai (ideate, prototype, feedback, refine) jo Project ke andar chalta hai, aur sab se zaroori skill yeh pehchanna hai ke masla description ka hai (behtar likho) ya feature ka (jaise calculation jo code se compute honi chahiye).

Aap ki baat sahi hai:

Ideate mein AI options banata hai. Yeh wohi synthesis hai jo Part 1 mein parhi thi.
Aap un mein se ek chunte hain.
AI us ka prototype banata hai.
Aap feedback dete hain (“yeh theek karo, aisa karo”).
AI refine karta hai, aur loop dobara chalta hai.


## Concept 10: Kab cheez prompt-and-iterate se bahar nikal jati hai

**Concept 9 se link:** Concept 9 mein dashboard artifact banaya tha. Ab sawal yeh hai ke woh chhota tool kab "chhota" nahi rehta.

### Kahani

Dashboard ek team ki internal zaroorat ke liye bana tha aur theek chal raha tha. Chhe mahine baad teen departments har Monday usay kholte hain, aur ek department apne numbers board ki report mein daal deta hai.

Ab yeh bilkul alag cheez ban chuki hai, aur kisi ne yeh faisla kiya hi nahi.

### Escalation signal

**Escalation signal** ka matlab hai: **jab doosre log is cheez par depend karne lagein.**

Jab tak aap akeli use kar rahi hain, prompt se theek karna kaafi hai. Jab doosre log is par bharosa karne lagte hain, to yeh infrastructure ban jata hai, aur ab ise chahiye:
- uptime (hamesha chalta rahe)
- access control (kaun dekh sakta hai)
- koi insaan jise toot jaye to bulaya ja sake
- guarantee ke aaj bhi wohi karta hai jo March mein karta tha

Yeh kaam developer ya architect ka hai. **Escalate karna sahi jawab hai, nakami nahi.** Asli nakami yeh hai ke aap prompt se chalati rahein jabke doosre log is par depend kar chuke hain, kyunke kisi ne yeh moment mark nahi kiya.

### Aasan misaal

Aap ne ghar mein chhota sa Excel banaya jis mein monthly kharcha likhti hain. Jab tak sirf aap dekhti hain, koi masla nahi. Phir poora khandan us se budget decide karne lage, aur bhai us ke numbers bank ko dikhane laga. Ab woh Excel "aap ka chhota sheet" nahi raha, us mein ghalti ka nuksan sab ko hai. Ab usay kisi theek insaan se banwana chahiye.

### Do signals jo milte julte hain magar alag hain

| Aap ko kya nazar aaya | Matlab | Kahan jana hai |
|---|---|---|
| Doosre log ab is par depend karte hain | Yeh infrastructure hai, engineering chahiye | Developer ya architect |
| Maine yeh kaam teen baar ek hi tareeqe se kiya | Shape stable ho gayi, ab "manufacture" ho sakta hai | Course "From One-Off to Worker" |

Pehla **kaun exposed hai** ke baare mein hai. Doosra **kya tareeqa ab badalna band ho gaya** ke baare mein.

### Viva ke liye ek line

Jab doosre log kisi tool par depend karne lagein (escalation signal), to woh prompt-and-iterate se nikal kar infrastructure ban jata hai aur developer ya architect ke paas jana chahiye, aur yeh nakami nahi, sahi faisla hai.

## Concept 11: Bad output ki 4 wajahein, waqt se pehchanein

**Part 3 se link:** Ab tak banane ki baat thi. Part 4 mein dekhte hain ke output kharab aaye to **kya karein**.

### Aam ghalti

Output achha na aaye to log do kaam karte hain: "yeh tool is kaam ka nahi" keh kar chhor dete hain, ya bina soche cheezein badalte rehte hain. Dono mein woh ek sawal chhoot jata hai jo sab se zyada madad karta hai:

> **Masla pehli baar kab nazar aaya?**

Chaar wajahein dekhne mein ek jaisi lagti hain, magar waqt unhein alag kar deta hai.

### Chaar wajahein

| Masla kab dikha | Wajah | Matlab | Jaldi test (1 minute) | Hal |
|---|---|---|---|---|
| **Pehle jawab se hi ghalat** | **Under-specification** | Prompt mein woh cheez thi hi nahi jo chahiye thi | Prompt dobara parhein, kya missing cheez us mein hai? | Jo chhoot gaya woh likhein |
| **Shuru theek, phir kharab** | **Context overload** | Chat itni lambi ho gayi ke shuru ki instructions kamzor ho gayin | Naye chat mein instruction dobara dein, kya ab theek chalta hai? | Restart karein ya summary se shuru karein |
| **Ek hi qism ki ghalti baar baar** | **Wrong feature ya model** | Step ghalat tool ko diya gaya | Sahi feature ya taqatwar tier se ek baar chala kar dekhein | Feature ya tier badlein |
| **Pehle chalta tha, ab nahi** | **Stale configuration** | Setup ki koi cheez purani ho gayi (instruction, file, Skill) | Instruction ya knowledge file ki tareekh dekhein | Configuration update karein |

Misaalein:
- "Numbers thode ghalat hain" ka matlab calculation prose mein maangi gayi thi. Hal: code execution (Concept 3).
- "Gehrai wale kaam ka jawab sathi (shallow) hai" ka matlab speed wala tier chuna gaya.

### Do zaroori baatein

1. **Waqt sirf pehla andaza deta hai, jawab nahi.** Ek hi waqt ki kai wajahein ho sakti hain, is liye jaldi test se confirm karein. Test negative aaye to bhi waqt zaya nahi hua, ek sab se mumkin wajah rule out ho gayi.
2. **Stale configuration sab se khatarnak hai kyunke chupke se aati hai.** Baaqi teen apne aap ko zahir karti hain, yeh nahi. Misaal: pichli quarter ke figures knowledge base mein pare hain aur is quarter ki report unhein quote kar rahi hai, bilkul sahi format mein. Model ko pata hi nahi ke jo aap ne diya woh purana hai. Yeh Concept 7 ke unstaffed gate ka jorha hai: dono mein control sahi set hua tha, phir khamoshi se kharab hua.

### Viva ke liye ek line

Bad output ki chaar wajahein hain (under-specification, context overload, wrong feature ya model, stale configuration), aur unhein pehchanne ka sab se sasta tareeqa yeh hai ke dekhein masla pehli baar kab nazar aaya.

## Concept 12 (aasan aur short)

**Concept 11 se link:** Concept 11 mein seekha ke bad output ki 4 wajahein hoti hain. Concept 12 mein seekhte hain ke unhein **kis order mein check karein**: jo sab se sasta hai woh pehle.

**Order (5 steps):**
1. **Prompt dobara dekhein:** kya kuch likhna bhool gayi? (role, context, task, constraints, format)
2. **Chat bohat lambi to nahi ho gayi?** Ho gayi to naya chat shuru karein.
3. **Sahi feature ya model use hua?** Calculation ho to code execution, mushkil kaam ho to taqatwar model.
4. **Setup purana to nahi?** Instructions, files, Skills.
5. **Sab se aakhir mein:** kya yeh kaam is tool se ho hi sakta hai?

**Misaal:** Gaari start nahi ho rahi. Aap pehle dekhti hain petrol hai ya nahi, phir battery, phir engine kholte hain. Seedha "gaari kharab hai, bech do" nahi kehti. Wohi yahan hai: pehle sasta check, phir mehnga.

**Log kya ghalti karte hain:** Seedha step 5 par chale jate hain ("yeh AI se nahi hota") ya sab se taqatwar model lagate hain, jabke prompt mein hi kuch missing tha.

**Step 5 kab sahi hai:** Jab aap koi aisi cheez maangen jo tool kar hi nahi sakta, jaise "agle quarter ki exact sales figure". Tab task badlein (exact number ki jagah range maangein), lekin pehle upar ke 4 check karein.

**Viva ke liye ek line:** Output kharab ho to sab se sasta check pehle karein (prompt, chat ki lambai, feature ya model, setup), aur "yeh kaam ho hi nahi sakta" sab se aakhir mein kahein.

## Concept 13: Reaction ko instruction banayein

**Concept 12 se link:** Concept 12 mein seekha ke masla dhoondne ka order kya hai. Ab Part 5 mein seekhte hain ke masla mil jaye to usay **theek kaise karein**, taake dobara na aaye.

### Main baat

Jab output pasand na aaye to hum aksar sirf **reaction** dete hain: "bohat generic hai", "tone theek nahi", "point miss kar diya". Reaction batati hai ke aap ko kaisa laga. **Instruction** batati hai ke kya badalna hai, taake agla output alag aaye.

### Ek sawal jo reaction ko instruction banata hai

> **Yeh theek hone ke liye kya hona chahiye, aur setup ka kaunsa hissa isay control karta hai?**

| Reaction | Instruction | Kaunsa lever |
|---|---|---|
| "Bohat generic hai" | Audience ka naam likho aur woh ek kaam jo unhein karna hai | Prompt |
| "Tone ghalat hai" | Tone ka constraint daalo jo har draft par lage | Instruction |
| "Point miss kar diya" | Woh ek sawal pehle likho jis ka jawab output mein hona chahiye | Prompt |
| "Purana data use kar raha hai" | Knowledge base mein purani file badlo | Knowledge |

Lever teen hain: **prompt, instruction aur knowledge.**

### Misaal

Aap ne darzi ko kaha "kapre theek nahi bane." Yeh reaction hai, darzi kuch nahi badal sakta. Agar kaho "aasteen ek inch chhoti karo aur gala thora kholo", yeh instruction hai. Sirf "theek nahi" kehne se agli baar bhi andaza hi hoga.

### Yaad rakhein

Agar aap lever ka naam nahi le sakti (prompt ya instruction ya knowledge), to aap ki critique abhi bhi sirf reaction hai, aur agli koshish andaze se hogi jo revision jaisi dikhegi.

### Viva ke liye ek line

Reaction sirf batati hai ke kaisa laga, instruction batati hai ke kya badalna hai, aur reaction ko instruction banane ke liye poochein ke theek hone ke liye kya chahiye aur setup ka kaunsa lever (prompt, instruction ya knowledge) isay control karta hai.

.

Teen levers aap ne theek pakre hain. Bas har ek ka farq yaad rakhein:

| Lever | Kab use karein | Misaal |
|---|---|---|
| **Prompt** | Sirf **is ek request** ke liye | "Is baar audience ka naam likho aur ek action batao" |
| **Standing instruction** | **Har baar** ke liye rule | "Hamesha tone formal rakho" |
| **Knowledge** | Aisi file ya data jo AI ko **parhna** hai | Purani file hata kar nayi attach karna |

Aap ne "data attach kar do" kaha, woh knowledge hai. Bas yaad rakhein ke yeh tab kaam aata hai jab masla **purane ya kam data** ka ho, tone ya format ka nahi.

**Ek misaal:** "Output mein purani price aa rahi hai." Yeh reaction hai. Is ka lever knowledge hai, to instruction yeh hogi: "Price list ki purani file hata kar nayi attach karo."

**Ek line mein:** Reaction mat do, instruction do, aur batao ke woh prompt se hogi, standing instruction se, ya knowledge se.


## Concept 14: Fix kahan rakhein (rule, reference ya procedure)

**Concept 13 se link:** Concept 13 mein seekha ke reaction nahi, instruction deni hai, aur teen levers hain. Ab sawal yeh hai ke fix mil jaye to usay **kahan rakhein** taake kho na jaye.

### Masla

Fix mil gaya, magar sirf us chat mein diya. Agle Monday ya jab koi aur kaam sambhale, wohi ghalti dobara aati hai aur wohi mehnat dobara karni parti hai.

### Test

> **Kya yeh correction dobara chahiye hogi, mujhe ya kisi aur ko?**

Haan to usay chat se nikal kar **configuration** mein daalein. Is ko **promotion** kehte hain.

### Teen ghar

Fix ko pehchanne ka ek sawal: yeh **rule** hai, **reference** hai, ya **procedure**?

| Fix kya hai | Matlab | Ghar | Misaal |
|---|---|---|---|
| **Rule** | Aisi limit jo hamesha lagti hai | Standing instruction | "Pehli line mein target segment likho" |
| **Reference** | Cheez jo kaam ko parhni hai | Knowledge base | Brand voice guide, current product list |
| **Procedure** | Steps ka silsila | Skill | "Weekly report is exact format aur order mein banao" |

### Galat ghar mein rakhein to kya hota hai

- Procedure ko ek line ki instruction bana do, to steps aur order kho jate hain.
- Reference material standing instruction mein thoons do, to har prompt bhari ho jata hai, chahe us run mein zaroorat ho ya na ho.

### Course ki do logon ki kahani

- **Marketer** ne dekha ke briefs mein target segment missing hota hai. Usne do standing instructions Project mein likh deen. Ab Project kholne wale har insaan ko theek draft milta hai.
- **Analyst** ko pata tha ke revenue report mein canceled orders nikalne hain, magar woh har mahine chat mein yaad dilata tha. Do hafte ki chhutti par gaya, colleague ne report chalayi, aur canceled orders ke saath numbers chale gaye. Fix mojood tha, bas aisi jagah tha jahan sirf ek insaan dhoond sakta tha.

### Memory kaafi kyun nahi?

AI ki memory sirf **aap ki** hoti hai, colleague ko nahi milti. Aur woh **best-effort** hai: kabhi yaad rakhta hai, kabhi nahi, aur aap usay khol kar parh nahi sakti. Configuration woh shared jagah hai jo sab khol kar dekh sakte hain, is liye us par bharosa karein.

### Aasan misaal

Aap ki dukaan mein ek rule hai "udhaar sirf purane customer ko". Agar sirf aap ko yaad hai, to chhutti par naya munshi udhaar de dega. Dukaan ke board par likh dein to har munshi ke liye rule wahi hai. Standing instruction wohi board hai.

### Viva ke liye ek line

Jo fix dobara chahiye hogi usay chat mein na chhoren, configuration mein daalein: rule standing instruction mein, reference knowledge base mein, aur procedure Skill mein, kyunke galat ghar mein rakhi fix kho jati hai ya bojh ban jati h

H

| Ghalti | Kahan badlein |
|---|---|
| Tone ya koi rule toot raha hai | **Standing instruction** |
| Purani info aa rahi hai (stale data) | **Knowledge base** mein naya data |
| Ek hi process har baar alag tareeqe se ho raha hai | **Skill** |

Teesre ke liye ek choti si baat: Skill is liye sahi hai ke woh process **har baar, har insaan ke liye ek hi tarah** chalta hai. Alag alag tareeqe se hona hi us ki nishani hai ke steps aur order kahin likhe hone chahiye.

Yeh Concept 12 se bhi juda hai. Wahan "stale configuration" ek wajah thi, aur yahan us ka hal knowledge base mein naya data daalna hai.

**Ek line mein:** rule ka masla to standing instruction, purane data ka masla to knowledge base, aur alag alag tareeqe ka masla to Skill.








## Concept 15: Friction dhoondein, phir optimize karein

**Concept 14 se link:** Concept 14 mein seekha ke fix ko sahi ghar mein rakhein. Ab sawal yeh hai ke **kaunsi cheez** ghar mein rakhni hai? Jawab: woh chhoti baar baar wali mehnat jo hum ne notice karna chhor di hai. Isay **friction** kehte hain.

### Friction kya hai?

Ek chhota kharcha jo har baar hota hai aur ab nazar nahi aata. Do minute ki reformatting kisi ko buri nahi lagti, magar saal mein 50 baar hoti hai.

### Teen nishaniyan

| Nishani | Kaisi dikhti hai | Hal |
|---|---|---|
| **Repetition** | Har baar wohi cheez paste ya type karti hain | Saved context ya standing instruction |
| **Correction** | Har output mein wohi flaw theek karti hain | Configuration badlein taake aaye hi nahi |
| **Variance** | Alag log wohi kaam karein to alag natija aaye | Shared Skill ya knowledge base |

**Variance sab se zyada chhoot jati hai**, kyunke kisi ek insaan ko feel nahi hoti. Farq sirf logon ke beech hota hai aur reviewer ko nazar aata hai.

### Friction na dikhe to?

Workflow ek baar chalayein aur har manual step likhte jayein. Woh list aap ka backlog hai.

### Friction hatane ke do tareeqe (is order mein)

1. **Consolidate:** steps ko jod dein. Teen prompts jinhein same background chahiye, woh asal mein ek prompt hain.
2. **Promote:** jo baar baar wala pattern bacha, usay configuration mein daalein (Concept 14).

Order is liye ke jis step ko aap merge karne wali thi, usay promote karna zaya mehnat hai.

### Course ka example

Weekly report mein har analyst ke 45 minute lagte the aur outputs alag aate the. Audit mein teen frictions nikle, aur Concept 14 ke test se sort hue:

| Friction | Qism | Ghar |
|---|---|---|
| Har analyst wohi background paste karta hai | Reference | Shared knowledge base |
| Report ka format haath se theek hota hai | Procedure | Skill |
| Har analyst alag issues pakarta hai | Rule | Standing instruction |

Natija: 45 minute se taqreeban 25 minute, team mein ek jaisa format, aur ek revision round kam.

### Aasan misaal

Aap roz subah dukaan ka hisaab ek hi tarah copy mein likhti hain aur har baar wohi columns banati hain. Pehle ek printed register bana lein (promote), aur agar do alag copies mein likhti hain to ek hi mein jod dein (consolidate).

### Viva ke liye ek line

Friction woh chhoti baar baar wali mehnat hai jo ab nazar nahi aati, aur tab pakri jati hai jab repetition, correction ya variance dikhe, phir pehle steps jodein (consolidate) aur baqi pattern configuration mein daalein (promote).

## Concept 16: Badalne se pehle naapo

**Ghar ka example:** aap kehti hain "maine chai ka naya tareeqa nikala, ab jaldi banti hai." Ammi poochti hain "kitni jaldi?" Agar aap ne pehle waqt naapa hi nahi tha, to aap jawab nahi de sakti.

## Teen cheezein, bas

```
1. Pehle naapo (Baseline)
   Naya tareeqa lagane se PEHLE likho: kitna waqt laga?
   Maslan: 45 minute

2. Phir badlo, phir dobara naapo
   Ab: 25 minute
   Ab aap keh sakti hain "45 se 25 minute"

3. Dono saath chalao (Parallel run)
   2-3 baar purana aur naya dono chalao,
   taake pata chale naya waqai behtar hai
```

## Pehle naapna kyun zaroori hai?

Baad mein aap purane tareeqe ka andaza lagayengi, aur woh hamesha **behtar** lagega, to asli farq nazar nahi aayega. Isi liye baseline pehle banti hai, baad mein nahi ban sakti.

## Parallel run kyun?

```
Naya theek nikla    --> poori tarah apna lo
Naya theek nahi     --> purana tareeqa maujood hai (fallback)
```

Aur jin logon ka kaam badla, unhein bhi dikhta hai "humne dono chalaye, yeh nateeja hai", sirf "tumhara kaam badal diya" nahi.

## Viva ke liye ek line

> Badalne se pehle baseline naapo (waqt, revision rounds, manual steps), phir badal kar dobara naapo, aur 2-3 round purana aur naya saath chala kar dekho ke naya behtar hai ya nahi.
## Concept 17 ka maqsad: ghalti hone se pehle plan tayyar rakho

**Ghar ka example:** aag lagne se pehle fire extinguisher kahan hai, yeh pata hona chahiye. Aag lag jaye tab dhoondne lage to der ho jati hai.

Concept 17 yehi kehta hai: **design kitna bhi achha ho, kabhi na kabhi bura output nikalega.** Is liye pehle se tay kar lo ke us waqt kya karna hai.

```
Ghalti hone se PEHLE (designer tay karta hai):
  1. Stop  --> Workflow kaise rokenge, kaun rokega?
  2. Scope --> Kitne outputs ghalat gaye, kahan gaye?
  3. Tell  --> Kis ko batana hai, kab tak?
  4. Map   --> Map mein kya badlenge?

Ghalti hone ke BAAD:
  Seedha yehi plan chalao, sochne mein waqt zaya nahi
```

## Plan na ho to kya hota hai?

```
Plan nahi:  Sab ghabra jate hain, jawab sust aur defensive hota hai
Plan hai:   Pehla ghanta seedha kaam mein guzarta hai
```

Course ki ek line: **jo team keh sake "jab workflow ghalat ho to hum yeh karte hain", usay workflow chalane ki ijazat milti hai.**

## Viva ke liye ek line

> Concept 17 ka maqsad hai ke bura output nikalne se pehle designer stop, scope, tell aur map ka plan tay kar le, taake ghalti hone par jawab fauri aur saaf ho.

Aap ne sahi pakra. **Course Concept 17 mein sirf yeh batata hai ke designer pehle se kya tay karey, poora step-by-step procedure nahi.** Course ke text mein jo "kaise" hai, woh yeh hai:

```
1. STOP
   Pehle se tay karo: workflow rokne ka sab se tez tareeqa kya hai,
   kaun rok sakta hai, aur kya usay kisi se ijazat leni parti hai?
   Agar jawab "jis ne banaya usse poochna parega" ho, to pehle yeh theek karo.

2. SCOPE
   Dekho kitne outputs affect hue aur kahan gaye.
   (Stale configuration ho to jis din se purani hui, us din se
   har result ghalat hota hai.)

3. TELL
   Pehle se likh lo: customer, internal owner, aur risk ya
   compliance team (agar ho). Kis ko, kab tak.

4. MAP
   Poochho: chaar causes mein se kaunsa tha? Step ghalat classify hua tha,
   ya sahi tha magar gate staffed nahi tha?
   Map mein badlo aur date likho.
```

Ek zaroori baat: course "scope kaise nikalte hain" ya "map mein exact kya likhte hain" ka koi detailed tareeqa nahi deta. Woh sirf yeh sawal batata hai. Poora **pehle ghante ka procedure** (rokna, facts record karna, apne organization ke raaste se report karna) **Governance, Risk & Responsible Use** course mein hai, jo maine abhi parha nahi.

**Ghar ka example (sirf samjhane ke liye, course ka nahi):**

```
Ali ka menu AI ne banaya, ek mehman ko gosht wala khana mil gaya.

Stop  : Baaqi khana serve karna rok do
Scope : Poochho aur kis kis ko ghalat khana gaya
Tell  : Us mehman se maafi, ammi ko batao
Map   : Menu plan mein "parhez ki list check" ka step likho, aaj ki date ke saath
```





