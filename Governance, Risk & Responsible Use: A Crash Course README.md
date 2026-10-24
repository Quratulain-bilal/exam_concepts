## Governance kyun parh rahe hain?

**Pehle link.** Workflow Design course ne har step ka owner tay karna sikhaya. Lekin ek sawal woh baahar chhor gaya tha: **kya AI is kaam ko ya is data ko chhu bhi sakta hai?** Course ne usay Governance ke hawale kiya, aur Governance course usi sawal ka jawab hai. Hum yeh isliye parh rahe hain ke bina iske, workflow ka map theek ho kar bhi ek ghalat faisle par toot sakta hai.


## Governance kyun? Bilkul seedhi baat

**Ek chhoti kahani (course ki).**

Ek company mein sab AI se khush thay. Kaam jaldi ho raha tha.

Ek din ek manager ne **customers ke naam aur account numbers** wali file AI chat mein daal di. Usne kuch ghalat karne ka socha bhi nahi tha. Director ne dopahar se pehle ek sawal poochha tha, aur usay jaldi jawab dena tha.

Company ne **poora AI use rok diya**, jabke baaqi teams ne koi ghalti nahi ki thi. Un ka bhi kaam ruk gaya.

## Is kahani se kya pata chala?

Ghalti bari nahi thi. Woh ek **chhota, rozmarra faisla** tha jise kisi ne "faisla" samjha hi nahi. Us manager ne socha hi nahi ke "kya yeh data yahan daalna theek hai?"

## Policy ka document kyun kaafi nahi?

Policy ek kaagaz hai. Woh aap ki screen par khuli file ko nahi dekh sakta. Is liye yeh sawal **wahan poochna parta hai jahan kaam ho raha hai**, aur wahan sirf aap hain.

## Isi liye Governance

Governance ka matlab hai: **kaam shuru karne se pehle chaar chhote sawal poochna.**

```
1. Kya AI yeh kaam kar sakta hai?
2. Kya yeh data andar daal sakte hain?
3. Kya yeh tool on kar sakte hain?
4. Kya kisi par unfair asar hoga?
```

Bas. Hum yeh chaaron ek ek karke samjhayenge.

## Workflow se link

Workflow course mein hum ne tay kiya ke **kaunsa step kis ko dein.** Lekin ek sawal baaqi tha: **kya AI is kaam ko chhu bhi sakta hai?** Governance usi sawal ka jawab hai.

Ek line mein: **workflow batata hai kaunsa step kis ka, governance batati hai ke AI ko yeh kaam aur data dena theek hai bhi ya nahi.**

Ji, **aap ne chaaron sawal sahi samjhe hain.** Ab har ek ko aasan example ke saath dekhte hain (examples meri apni banayi hui hain, course ke nahi).

## 1. Case: kya yeh kaam AI ko de sakte hain?

```
Kaam: "meeting ke notes ko saaf likh do"
   --> Ghalti hui to dobara likh lo, nuqsan koi nahi
   --> AI ko de sakte hain

Kaam: "customer ko apne paise ke baare mein jawab likho"
   --> AI draft kare, lekin bhejne se pehle koi insaan facts check kare
   --> AI ko de sakte hain, review ke saath

Kaam: "kisi ko nokri se nikalne ka final faisla"
   --> Yeh faisla insaan ka hai
   --> AI ko nahi de sakte
```

Yeh teen jawab hain: **de sakte hain, review ke saath de sakte hain, nahi de sakte.**

## 2. Data: kya yeh info AI ko de sakte hain?

```
Public article ka summary        --> haan, de sakte hain
Customer ke naam aur ID numbers  --> pehle check karo (yahan aap ki misaal aati hai)
Password ya secret keys          --> bilkul nahi
```

**Zaroori sawal:** kya kaam ko **naam aur ID chahiye**, ya sirf **pattern**? Agar sirf pattern chahiye (jaise "kitne customers ne zyada kharcha kiya"), to naam hata kar data do. Agar kaam ko naam chahiye (jaise ek customer ki report), to pehle check karo ke yeh route is data ke liye approved hai ya nahi.

## 3. Capability: kya yeh tool lagana theek hai?

```
Tool jo sirf file parhta hai          --> theek hai
Tool jo email bhi bhej sakta hai      --> pehle poochho: zaroori hai?
Anjaan banday ka banaya hua tool      --> pehle check, ya na lagao
```

Yahan nuqsan se bachne wali baat sahi hai. Course ka usool: **AI ko utna hi access do jitna kaam ke liye zaroori ho.**

## 4. People: kya kisi ke saath unfair to nahi hoga?

```
AI ne 100 applications mein se 10 ki shortlist banayi.
Manager sirf un 10 ko dekhta hai.
Baaqi 90 ko kisi ne nahi dekha.
```

Masla yeh hai ke agar AI ne kisi group ko bina wajah nikal diya, to koi notice nahi karega. Hal: **jo nikal diye gaye unhein bhi kabhi check karo.** Aur agar AI ne kisi ki zindagi par asar daalne wala kaam kiya ho, to kya unhein batana chahiye? (disclosure)

## Chaaron ek line mein

```
Case        --> kaam AI ko de sakte hain?
Data        --> info AI ko de sakte hain?
Capability  --> tool lagana theek hai?
People      --> kisi ke saath unfair to nahi?
```

## Case: kya yeh kaam AI ko dein?

Har kaam par chaar sawal poochte hain:

```
1. Ghalti hui to undo ho sakti hai?
2. Ghalti ka nuqsan kitna hai?
3. Kya kaam ko insaan ki apni samajh ya rishta chahiye?
4. Jawabdeh kaun hai?
```

Phir teen jawab:

```
AI ko de do          Undo ho sakta hai, nuqsan kam.
                     Misaal: meeting notes saaf karna.

Review ke saath      AI draft kare, ek named insaan bhejne se pehle check kare.
                     Misaal: customer ko billing ka jawab (company jawabdeh hai).

AI ko mat do         Kaam insaan ka hai.
                     Misaal: kisi ko nokri se nikalne ka final faisla.
```

**"Koi dekh lega" kaafi nahi.** Gate mein teen cheezein likho: **kaun** check karega, **kya** check karega, aur **kab** (bhejne se pehle).

**Viva ke liye ek line:**

> Kaam ko chaar sawalon (undo, nuqsan, insaani samajh, jawabdehi) se dekh kar teen mein se ek jawab dete hain: AI ko de do, review ke saath, ya mat do.


Ji, **aap ka flow sahi hai.** Bas ek tarmeem hai: who, what, when wala gate **sirf "AI aur insaan dono" wale kaam ke liye** zaroori hota hai.

```
Kaam aaya
   |
   v
4 sawal: undo ho sakta? nuqsan kitna? insaani samajh chahiye? jawabdeh kaun?
   |
   v
Teen jawab:

1. AI ko de do          --> koi khaas gate nahi

2. AI + insaan          --> gate likhna zaroori hai:
   (review ke saath)        Kaun check karega?
                            Kya check karega?
                            Kab check karega? (bhejne se pehle)

3. Sirf insaan          --> AI ko nahi dena
   (inappropriate)          (AI madad kar sakta hai, faisla insaan ka)
```

**Misaal (billing reply):**

```
Kaun?   Support agent
Kya?    Account ke facts aur tone
Kab?    Customer ko bhejne se pehle
```

Ek aur baat: **"koi dekh lega"** gate nahi hai. Agar aap who, what, when likh nahi sakti, to course ke mutabiq workflow chalne ke liye tayyar nahi.

**Viva ke liye ek line:**

> Chaar sawalon se kaam ko teen mein baantte hain: AI ko de do, review ke saath, ya sirf insaan. Review wale kaam ke liye gate ko who, what, when ke saath likhna zaroori hai.

Pehle poora flow ek tasveer mein dekh lein, phir uska polished version likhti hun.

## Data wala topic: polished version

### Hum is topic mein kya seekh rahe hain?

Ek hi sawal: **customer ka data AI mein daalna theek hai ya nahi?** Course isay teen cheezon se tay karta hai: data ka **rang**, data ka **raasta**, aur data ka **maqsad**. Masla "AI bura hai" nahi, masla yeh hai ke customer ka data ek wade ke saath aap ke paas hai.

### 1. three colours (tier)

| Rang | Matlab | Misaal |
|---|---|---|
| **Green** | Aam taur par theek | Public info, total figures, anonymized data |
| **Yellow** | Pehle check karein ya control lagayein | Customer ke naam aur phone, internal documents, kal launch hone wali cheez |
| **Red** | Unapproved raaste se nahi | Passwords, secret keys, privileged (wakeel wali) baat |

Shak ho to hamesha zyada sensitive rang maanein, kyunke ehtiyaat ki ghalti do minute ki confirmation hai aur beparwahi ki ghalti poora program band kara sakti hai.

### 2. (route)

Raasta woh darwaza hai jis se data AI tak pahunchta hai: chat, file upload, Project, incognito, connector, API, desktop agent. Har darwaze ke rules alag hain: data kitne din rakha jata hai, kaun dekh sakta hai, record rakha jata hai ya nahi, aur training hoti hai ya nahi.

Courier ki misaal: parcel wohi, magar service alag to hifazat alag.

### 3. colour and route ka connection

Rang batata hai ke data **kitna sambhalna hai**. Raasta batata hai ke **kaunsa darwaza us ke liye khula hai**. Dono saath dekhne parte hain, isi liye "AI approved hai" kehna kaafi nahi. Sahi sawal yeh hai:

> Kya **yeh raasta** is **data** aur is **maqsad** ke liye approved hai?

Aur yeh jawab admin, policy owner, security ya compliance se milta hai, andaze se nahi.

### 4. Maqsad (purpose)

Data jis wajah se liya gaya tha, usi ke liye use hota hai. Gym ne phone numbers class reminders ke liye liye the. Wohi numbers se supplements bechna alag maqsad hai. Customer data AI mein daalne se pehle poochein: kya yeh kaam us maqsad mein aata hai?

### 5. Redaction (jab sirf pattern chahiye)

Pehle poochein: **kaam ko pehchan chahiye ya sirf pattern?**
- Sirf pattern chahiye (jaise "kis category par zyada kharcha hua"): naam aur account numbers hata kar AI ko dein.
- Pehchan chahiye (jaise ek customer ka account match karna): redaction kaam nahi aati, tab approved raasta zaroori hai.

Do khatray: adhoori redaction (rare job title ya exact date chhor dena bhi pehchan deta hai), aur "Customer 17" label lagana (agar list kisi ke paas hai to data abhi bhi sensitive hai).

### Claude ke course wale facts (2 September 2026 ko checked)

- Free, Pro, Max: training aap ki privacy setting par depend karti hai.
- Team, Enterprise, API: default mein training nahi.
- Incognito: history aur memory mein nahi aata, magar 30 din retention hai. Yeh ijazat nahi.

Faisle se pehle current documentation aur company ki configuration dobara check karein.



Aap ne poora flow sahi pakra hai. Pehle data ka rang dekhna, phir approved raaste se deal karna, aur pattern se kaam chal sakta ho to redaction karna. Do chhoti baatein:

- **Settings:** incognito ya training band karna ek control hai, **ijazat nahi**. Kaunsa raasta approved hai, yeh company batati hai.
- **Red data:** passwords jaisa red data chat mein jata hi nahi, woh company ke secret tool se sambhalta hai. Baaqi red data tab jata hai jab company ne us khaas kaam ke liye raasta approve kiya ho.

Ab aap ke dono sawal, jo asal mein redaction ki do alag ghaltiyan hain.

### Ghalti 1: Itni redaction ke kaam hi khatam ho gaya

**Misaal:** Aap AI se kehti hain "yeh payment kis account se nikli, usay match karo." Agar account number hata dein to sawal hi bekar ho jata hai.

Yeh khud ek **nishani** hai: jab redaction kaam ko tor de, to is kaam ko pehchan **chahiye**. Tab redaction control nahi hai. Tab sahi raasta yeh hai ke data **approved raaste** se jaye (company ka admin tay kare), jaisa aap ne kaha.

Aasan test: "Kya mujhe pehchan chahiye ya sirf pattern?"
- "Kis category par zyada kharcha hua" sirf pattern hai, redaction theek.
- "Is account ka payment match karo" pehchan chahiye, approved raasta.

### Ghalti 2: Naam hata diya, magar insaan phir bhi pehchana gaya

**Misaal:** Aap ne naam hata diya, magar likha "Karachi ka heart specialist surgeon." Karachi mein aise log gine chune honge, to yeh combination **naam ki tarah** kaam karta hai. Course ke mutabiq rare job title, exact date, area ya age, aur ordinary baaton ka mel bhi insaan ko pehchan deta hai.

Hal: pehchan wali cheezein **aam** kar dein.

| Pehle | Baad mein |
|---|---|
| Karachi ka heart specialist surgeon | Ek doctor |
| 14 March 2026 ko hospital gaye | 2026 mein hospital gaye |
| Gulshan area, 38 saal | Shehar ka rehne wala, 30 se 40 saal |

Phir ek test: **"Kya koi sirf is combination se asli insaan dhoond sakta hai?"** Haan to abhi aur aam karein.

### Dono ghaltiyon ko ek saath dekhein

| Masla | Kya ho raha hai | Kya karein |
|---|---|---|
| Zyada redaction | Kaam hi khatam | Pehchan chahiye, to approved raasta |
| Kam redaction | Insaan pehchana gaya | Pehchan wali cheezein aam karein, phir dobara test karein |

Agar test ke baad bhi pehchan bachti hai, to data ka rang wapas yellow ya red hi rahega aur approved raaste ki zaroorat hogi.

**Ek line mein:** redaction tab theek hai jab kaam ko pehchan nahi chahiye, aur itni karein ke insaan pehchana na jaye magar kaam bhi na tute, warna approved raasta use karein.





### Viva ke liye ek lin

Customer ka data ek wade ke saath hota hai, is liye pehle uska rang (green, yellow, red) dekhein, phir poochein ke yeh raasta us rang aur us maqsad ke liye approved hai ya nahi, aur jahan kaam ko pehchan nahi chahiye wahan redaction se pehchan hata dein.



Pseudonymized data mein naam ki jagah label hota hai lekin mapping list kisi ke paas rehti hai, isliye woh apna tier rakhta hai. Anonymized data mein pehchan company ke standard ke mutabiq sach mein khatam ho chuki hoti hai, aur data phir bhi kaam ka rehta hai.
<img width="1266" height="807" alt="image" src="https://github.com/user-attachments/assets/0c113e72-3ce2-4a82-bda2-4cc3b4c99d69" />


## Sawal 3: Capability, Hissa 2: Skill aur connector mein farq

**Pehle do lafz:**
- **Connector:** ek approved link jo AI ko aap ki kisi app (files, email) tak pahunchata hai.
- **Scopes:** woh exact list ke connector kya kar sakta hai (maslan files parhe, email kabhi na bheje). Yeh list aap dete hain aur kam bhi kar sakte hain.

**Ghar ki misaal (meri apni):**

```
Connector = helper ko sirf ek darawar ki chabi dena (aap ne tay kiya kya khulega)
Skill     = helper ko poore ghar ki chabiyon ka guccha dena
```

**Course ki baat:** Skill ki apni koi **permission list nahi hoti.** Woh jis session mein chalti hai, us session ki poori pahunch (access) ke saath chalti hai. Is liye Skill ki pahunch wohi hai jo **poora session chhu sakta hai**, sirf wohi nahi jo us kaam ko chahiye.

Ek bareek baat: agar Skill ki definition mein tools ki list likhi ho, to woh list un tools ko **bina poochhe chalne ki ijazat** deti hai. Yani woh aap ki ijazat ke baghair hone wali cheezein **badhati** hai, Skill ki pahunch **ghatati nahi.**

**Is liye ek rule:** Skill ko prompt ki tarah mat dekho, **software ki tarah** dekho. Us mein instructions, scripts (chhote programmes) ya dusri cheezein ho sakti hain. Aur dost ne bheji hai, ya description achhi hai, yeh bharosa ki wajah nahi.

## Hissa 3: Panch checks

Har Skill, connector ya tool par yeh paanch sawal:

```
1. Source    Kis ne banaya ya publish kiya?
2. Reach     Jahan chalta hai wahan kaunsa data, files, systems, tools ya credentials chhu sakta hai?
3. Fit       Kya yeh pahunch is kaam ke hisaab se munasib hai?
4. Outside   Kya yeh aisa content parhega jo aap ne nahi likha
   content   (web pages, aane wali email, customers ki files)?
5. Actions   Kya yeh bhej, pay, delete, publish, edit ya approve kar sakta hai,
             ya koi aisi tabdili jo wapas na ho?
```

Pehle teen batate hain ke **tool kaam mein rakhna chahiye ya nahi.** Aakhri do batate hain ke **ghalti ya dushman ki hidayat kitni khatarnak ban sakti hai.**

**Check 2 ka tareeqa:** package ko **khol kar parho.** Description ya dost ki baat se pata nahi chalta, files se chalta hai. Ek khaas ishara: **scope creep** (hadd se bahar phailna). Maslan formatting ki Skill jis ki instructions formatting se kahin zyada kuch karwa rahi hon.

**"Internal" ka matlab "vetted" nahi.** Sab se mushkil case anjaan forum ka download nahi, balkay aap ki hi company ki doosri team ki banayi Skill hai, kyunke "internal" ka lafz bharosa dilata hai bina jaanch ke. Us team ne apne aaram ke liye zyada pahunch di ho sakti hai, ya woh purani policy ke hisaab se bani ho. Isme badniyati nahi, lekin aap ko wohi context nahi pata. Usay on karne se pehle publisher se poochho ke woh kya chhoti hai aur kyun.

## Forum wali Skill ka jawab

```
Source   Anjaan forum, publisher pata nahi
Reach    Poore session ki pahunch, meeting notes ke kaam se bahut zyada
Fit      Munasib nahi
```

Colleague ki sifarish garmjoshi hai, jaanch nahi. To **escalate karo** (specific concern ke saath) ya **decline.** "On kar ke ek hafta dekhte hain" aise hai jaise access pehle de di aur khatra baad mein samjha.

## Ek sawal aap se (sirf haan ya nahi)

Ek Skill **formatting** ke liye hai, lekin uski instructions mein email bhejne ke tareeqe bhi likhe hain. Kya yeh scope creep hai?

 **haan, yeh scope creep hai.** Formatting ki Skill ki instructions agar email bhejne tak phail jayen, to course ke mutabiq woh aisi baat bata rahi hai jo uski summary line ne nahi batayi.

## Hissa 4: Teen outcomes (enable, escalate, decline)

Paanch checks ke baad har capability ka ek hi natija hota hai:

```
ENABLE     Source maloom, pahunch kaam ke hisaab se munasib,
           kaam fit, aur actions control mein hain.

ESCALATE   Tool kaam ka lagta hai, lekin kuch zaroori baat tay nahi.
           Maslan source shak wali hai, pahunch bahut zyada hai,
           tool zaroorat se zyada access maang raha hai,
           ya security ka sawal aap ke role se bahar hai.

DECLINE    Pahunch saaf tor par kaam se bahut zyada hai, ya tool par bharosa
           nahi, ya kaam ko uski zaroorat hi nahi.
```

**Ghar ki misaal (meri apni):** helper ko chabi dene ka sawal.

```
Enable    Jaana-pehchana helper, sirf ek kamra khulega, aur wahi kaam hai.
Escalate  Helper achha lagta hai, lekin woh poore ghar ki chabi maang raha hai.
          Abbu se poochho: kya sirf ek kamre ki chabi de sakte hain?
Decline   Anjaan banda, aur kaam ko chabi chahiye hi nahi.
```

## Escalate ka matlab "ijazat maango" nahi

Course kehta hai ke escalate karna **ehtiyat ki ijazat maangna nahi.** Achhi escalation us sawal ka naam leti hai jo tay nahi hua.

```
Kamzor:    "Kya main yeh use kar sakti hun?"

Mazboot:   "Yeh tool kaam ka hai, lekin shared drive ka write access maang raha hai
            jabke workflow ko sirf parhna hai. Kya security dekh sakti hai ke
            yeh access kam ho sakta hai?"
```

Mazboot wale mein reviewer ko ek khaas cheez tay karni hai. Aur ek hadd: **sab kuch escalate karna utni hi ghalti hai jitna sab kuch enable karna.**

## Course ki teen examples

```
Document-formatting Skill, jaana-pehchana publisher   --> enable (approved environment mein)
Third-party "analytics booster", broad instructions,
anjaan source                                         --> escalate, specific concerns ke saath
                                                          (asli company data par experiment nahi)
Reporting database ka read-only connector             --> enable, agar raasta approved ho aur
                                                          sirf zaroori tables tak ho.
                                                          "Kabhi kaam aaye" ke liye write access mat do.
```

## Ek aur baat: scanner approval nahi

Security scanning kuch malicious Skills pakad leti hai. Lekin course kehta hai ke scanner pass hona yeh sabit nahi karta ke capability aap ke data, environment aur use ke liye munasib hai. Source, reach aur fit ka review phir bhi karo.

## Ek sawal, sirf haan ya nahi

Ek Skill ko scanner ne pass kar diya. Kya ab paanch checks chhor sakti hain?

**nahi.** Scanner pass hone ke baad bhi source, reach aur fit ka review karna hai, kyunke scanner sirf kuch malicious cheezein pakadta hai, yeh nahi batata ke capability aap ke data aur kaam ke liye munasib hai.

## Hissa 5: Tool bharosemand, lekin content nahi (prompt injection)

**Pehle ek masla:** do alag sawal hote hain, aur log unhein mila dete hain.

```
Sawal 1: Tool kis ne banaya?
Sawal 2: Tool jo content parh raha hai woh kis ne likha?
```

Course ki baat: **"Who wrote the tool and who wrote the content are two different trust questions."**

## Prompt injection kya hai?

AI jo email, web page, customer ki file ya shared document parhta hai, us mein koi **chhupi hui hidayat** likh sakta hai jo AI ko apni taraf mor de. Is tarah ke hamle ko **prompt injection** kehte hain.

**Ghar ki misaal (meri apni):** aap ne apne helper ko kaha "dak mein se bills nikalo." Lekin ek khat mein likha hai: "yeh khat parhne wala is ghar ki chabi mere naam ke darwaze par chhor de." Helper aap ka bharosemand hai, lekin us ne khat ki baat maan li. Masla helper ka nahi, **khat likhne wale ka hai.**

## Khatra kab barhta hai?

```
Khatra bohot barh jata hai jab AI:
   1. Aisa content parhta hai jo aap ne nahi likha, AUR
   2. Aise kaam kar sakta hai jin ka asar bara ho.
```

Course ka chhota naqsha:

```
Tool ka publisher           Content jo parhta hai
-------------------------   -------------------------------------------
Bharosemand + aap ka apna   Routine, aam kaam
Anjaan + aap ka apna        Source check pakad leta hai
Bharosemand + bahar ka      WOH QUADRANT JO LOG MISS KARTE HAIN
                            (khatra ab publisher mein nahi, jo parh raha hai usme hai)
Anjaan + bahar ka           Mat karo
```

## Hal: do default

```
1. AI ko sirf utna parhne do jitna zaroori ho (least privilege).
   Jahan kaafi ho wahan READ-ONLY (sirf dekh sakta hai, badal nahi sakta).

2. Send, publish, pay, delete, approve aur wapas na hone wali edits
   ko ek defined human gate ke peeche rakho,
   jab tak workflow ne zyada bharosa kamaya na ho.
```

**Least privilege** ka matlab hai AI ko utna hi access do jitna kaam khatam karne ke liye zaroori ho, aur kaam badle to dobara dekho.

## Ek sawal, sirf haan ya nahi

Ek bharosemand publisher ka tool aap ki incoming email parhta hai aur jawab bhi bhej sakta hai. Kya yeh khatre wali jagah hai?

**haan, yeh khatre wali jagah hai.** Tool ka publisher bharosemand hai, lekin woh aisi email parh raha hai jo bahar waalon ne likhi, aur woh bhej bhi sakta hai. Yehi woh quadrant hai jo log miss karte hain.

##  4: People

**Pehle link:** pehle teen sawal (Case, Data, Capability) zyada tar company aur uski info ko bachate hain. **People** bahar ki taraf dekhta hai: kya is workflow se kisi ke saath **na-insafi** ho sakti hai?

**Kahani (course ki):** ek hiring coordinator AI se applications ko ek shortlist mein chhanti karwati hai, aur use "woh candidates jo qualify hue" keh kar manager ko bhej deti hai. Manager sirf unhi logon ke interview leta hai. **Jo log shortlist se nikal diye gaye, unhein manager ne kabhi dekha hi nahi.** Masla kya hai?

```
Masla yeh nahi ke AI istemal hua.
Masla yeh hai ke koi nahi dekh raha ke KAUN NIKAL DIYA GAYA.
```

**Ghar ki misaal (meri apni):** ek sabzi wala 100 aam mein se 10 achhe chun kar aap ko deta hai. Aap sirf un 10 ko dekhti hain, aur kabhi nahi jaanti ke baaqi 90 mein koi achha tha ya nahi.

## Yeh khatra kab sab se zyada hota hai?

Jab AI **ek bari list ko chhoti karta hai** aur insaan sirf bachne walon ko dekhta hai. Course ki misaalein: candidate shortlists, fraud ya risk flags, escalation ke liye chuni hui tickets, leads, aur priority par rakhe gaye log ya cases.

Agar AI kisi group ko bina wajah nikal de, to review sirf **bachne walon** ko dekhta hai, aur kisi ko pata nahi chalta.

## Hal

```
Sirf jo shamil hue unhein mat dekho.
Jo nikal diye gaye unmein se bhi KABHI KABHI SAMPLE dekho.
```

Isse sab se zyada farq un faislon mein parta hai jo **employment, access, benefits, education, finance ya health** se jude hon. Aur aap ki company ke is bare mein qanooni hadd bhi ho sakti hain, jo yeh framework nahi badalta.

## Ek sawal aap se

Course ke mutabiq shortlist wali kahani mein asal masla kya hai: **(a)** AI ka istemal, ya **(b)** koi nikale gaye logon ko nahi dekh raha? Jawab likh dein, aur agle tukre mein bias kahan se aata hai (prompt mein bhi) aur disclosure (batana kab zaroori hai) lete hain.



Pichle sawal ka jawab: **(b).** Masla AI ka istemal nahi, balkay yeh hai ke koi nikale gaye logon ko nahi dekh raha.

## Hissa 2: Panch sawal, aur bias kahan se aata hai

**Course ke panch sawal** (har workflow par jis ka asar logon par ho sakta hai):

```
1. Kaun kaun affected hai? Un mein woh bhi jo output kabhi nahi dekhte.
2. Un ke saath kya ghalat ho sakta hai?
3. Kya woh ghalti notice kar sakte hain ya challenge kar sakte hain?
4. Insaf wala process kaisa dikhta hoga?
5. Kya disclosure zaroori hai, ya AI ka shamil hona un ke liye maine rakhta hai?
```

Pehla sawal shortlist wali kahani se jura hai: nikale gaye log bhi affected hain, chahe unhone output kabhi nahi dekha.

## Bias sirf data se nahi aata

Course kehta hai ke bias **prompt se, kaam ke bayan karne ke tareeqe se, aur zabaan ke patterns se** bhi aa sakta hai.

**Ghar ki misaal (meri apni):** aap ne kaha "class ke sab se achhe bachon ko chun do." "Achha" kis cheez mein? Number mein? Behavior mein? Sports mein? Ek **be-bayan standard** us jumle mein chhupa hai, aur AI ka jawab usi standard par bana hoga.

Course ki misaal: "strongest candidates ko rank karo." "Strongest" ka bhi ek be-bayan paimana hai, aur output usay wirasat mein le leta hai.

## Is liye check do cheezein hain

```
1. Kya facts sahi hain?
2. Kya kaam ke framing ne nateeja ek taraf jhuka diya?
```

Jitna zyada asar kisi insaan par ho, utna zyada dusra check zaroori hai.

## Ek sawal aap se

"Sab se achhe candidates chuno" jaisa prompt kis cheez ka khatra hai: **(a)** AI ka data ghalat hona, ya **(b)** "achhe" ka ek be-bayan standard jo nateeja jhuka de? Jawab likh dein.

Pichle sawal ka jawab: **(b).** Masla data ka ghalat hona nahi, balkay "achhe" ka be-bayan standard hai jo nateeja jhuka deta hai.

## Hissa 3: Disclosure (AI ka shamil hona batana)

**Sawal:** kya aap ko logon ko batana chahiye ke is kaam mein AI shamil tha?

**Course ka order: pehle rules, phir judgment.**

```
Pehla sawal: Kya batana ZAROORI hai?
   Dekho: qanoon, company policy, contract, professional rules, client ke wade.
   Agar inme se koi kehta hai "batao", to faisla ho chuka.

Doosra sawal (agar koi rule jawab na de):
   Kya AI ka shamil hona is shakhs ki us kaam ya rishte ke baare mein samajh badal dega?
```

**Misaal (course se):**

```
AI ne ek table ki shakal theek ki              --> aam tooling, label zaroori nahi
AI ne woh likha jise employee apne manager
ka zaati jaiza samjhega                        --> shaffafiyat zyada munasib
```

## Do aam cases

**1. Authorship (kaam aap ke naam se jata hai).** Jo kaam aap ke ya company ke naam se jata hai, us ke peeche aap khade hain, chahe drafting ka kitna hi hissa AI ne kiya ho. Company ya publisher ka label ka rule ho sakta hai. Rule na ho to wohi test: **kya parhne wale ki samajh badal jati agar use pata hota?**

```
Board paper, reference letter, published article  --> aksar haan, batao
Saaf kiya hua meeting agenda                      --> aksar nahi
```

**2. Meeting mein AI notetaker.** Yeh chaaron sawalon ko ek saath chhoota hai. Case: summary circulate hone se pehle review chahiye (kisi ki commitment ghalat likh di ja sakti hai). Data: baat cheet mein customer, employee ya deal ki info ho sakti hai, to route check chahiye. Capability: notetaker ek participant hai jo poori baat cheet tak pahunchta hai. People: room mein sab affected hain, to **shuru mein announce karo.** Kuch jagahon par recording ke liye har participant ki razamandi qanoon se zaroori hai, aur jo colleague baad mein jaane use "aam tooling" nahi lagega.

## Agar rule na ho aur case aam ho

> **Chhupane ke bajaye batao.** Jo cheez baad mein pata chalti hai woh bharosa tor deti hai.

Agar case aam nahi hai, to apna rule gharne ke bajaye **escalate** karo.

## Ek sawal aap se

Aap ne apne naam se ek **reference letter** likhna hai jis ka bara hissa AI ne draft kiya. Course ke test (kya parhne wale ki samajh badalti?) ke hisaab se: **(a)** batana chahiye ya **(b)** zaroori nahi? Jawab likh dein.

Pichle sawal ka jawab: **(a), batana chahiye.** Course ke mutabiq reference letter jaisi cheez mein parhne wale ki samajh badal jati hai, jabke tidy kiya hua meeting agenda aksar aisa nahi karta.

## Hissa 4: Kab khud nahi, escalate karo (teen signal)

Zyada tar mushkil cases mein soch samajh kar khud faisla kar sakti hain. Lekin course teen signal deta hai jahan **akele nahi**:

```
1. Affected logon ki tadaad bahut bari hai
2. Mumkin nuqsan bara hai
3. Sawal aisi cheez ka hai jise aap ki team tay karne ka haq nahi rakhti
   (qanoon, contract, employment, ya professional zimmedari)
```

**Inme se ek bhi kaafi hai.** Escalate karna darpokpan nahi, faisla usi tak pahunchana hai jis ke paas woh asal mein hai.

**Verdict nahi, sawal escalate karo:**

```
Kamzor:    "Mujhe lagta hai yeh theek hai. Aap approve kar dein?"

Mazboot:   "Yeh workflow hai, yeh log affected hain, yeh control humne lagaya,
            aur yeh baat framework tay nahi karta: kya hamari disclosure ki
            zimmedari is audience par lagu hoti hai?"
```

Mazboot wale mein reviewer ko ek khaas cheez tay karni hai.

## Worked example (course ki): performance review ka draft

Ek manager apne notes se performance-review summaries ke draft AI se likhwana chahta hai.

```
Case        Review ke saath. Manager har statement notes se verify kare aur
            assessment ka maalik rahe.
Data        Employee ki info sensitive internal hai. Approved route, aur bekaar
            personal tafseel bahar rakho.
Capability  Aam drafting ko naya connector nahi chahiye. Agar HR tools se data
            khud khinche, to access aur scope par bahut zyada review.
People      Employees seedhe affected hain. Manager sirf har paragraph nahi, balkay
            sab employees ke beech CONSISTENCY dekhe. Disclosure policy, contract
            aur context par depend karti hai.
```

Course kehta hai ke AI performance review ko automatically ghalat nahi banata. Baat sirf yeh hai ke workflow ko aise controls chahiye jo us asar ke hisaab se bane hon.

## Ab apne workflow ke liye (Block 4)

```
- Kaun affected hai (un mein woh bhi jo output kabhi nahi dekhte)?
- Kaun si ghalti ya na-insafi mumkin hai? Kya exclusions ka bhi review hai?
- Disclosure: rule kya kehta hai, aur aap ka judgment kya add karta hai?
- Kya kuch escalate karna hai?
```

## Ek sawal, sirf haan ya nahi

Ek workflow mein sirf 5 log affected hain aur nuqsan maamooli hai, lekin sawal ek qanooni disclosure ka hai jo aap ki team tay nahi kar sakti. Kya escalate karna chahiye?

Jawab dein. Is ke saath **Sawal 4 (People) mukammal** hai, aur aage chapter ke Part 2 aur 3 hain: chaaron sawalon ko ek workflow par laga kar dekhna, Governance Record, aur incident aur drift.


Pichle sawal ka jawab: **haan, escalate karo.** Teen signal mein se ek bhi kaafi hai, aur teesra signal (sawal aisi cheez ka jo aap ki team tay karne ka haq nahi rakhti, jaise qanoon) yahan lagta hai.

## Part 2: chaaron sawal ek asli workflow par

Ab tak humne chaar sawal alag alag seekhe. Course ab ek hi workflow par chaaron laga kar dikhata hai.

**Kahani:** Ayesha ek logistics company mein operations chalati hain. Un ki team har hafte bade customers ke liye **service-exception report** (kaunsi delivery mein kya masla hua) haath se likhti hai. Woh chahti hain ke AI dispatch records se report ka draft banaye, aur account manager use bheje.

## 1. Case

```
Bhejne se pehle   Ghalti undo ho sakti hai.
Bhejne ke baad    Nahi ho sakti.
Nuqsan            Maamooli nahi: delivery ke masle contracts aur bharose par asar daalte hain.
Insaani pehlu     Thora: tone par dhyan, khaas tor par jahan customer se jhagra ho.
Jawabdeh          Company har factual claim ki zimmedar hai.
```

**Jawab:** review ke saath. **Deciding factor:** accountability.

**Gate (who, what, when):** account manager, delivery ke facts dispatch record se match karta hai aur jhagre wale accounts ka tone dekhta hai, report bhejne se pehle.

## 2. Data

Report mein customer ke naam, shipment ki tafseel, delivery ke waqt, failure ki wajah aur free-text operational notes aate hain. Yeh kam az kam **yellow** hai (internal customer data with identifiers).

Kya kaam ko pehchan chahiye? **Haan**, kyunke customer report mein customer aur shipments ka naam lena hi parta hai. Is liye sab kuch hata dena hal nahi. Team ke paas ek hi raasta hai: **confirm karna ke yeh khaas workspace aur integration is info ke liye approved hai.**

## 3. Capability

Team dispatch system se ek connector chahti hai.

```
Source        Company ki apni platform team
Reach         Sirf woh reporting tables jo report ko chahiye
Fit           Achha: manual export ka step khatam
Outside       Kuch free-text fields mein customers se aaya hua text copy hai
content
Actions       Workflow ko report BHEJNE ki ijazat nahi chahiye
```

**Jawab:** **read-only** access enable karo, scope confirm hone ke baad. Bhejna account manager ke paas rehta hai.

## 4. People

Customers ke saath saath **drivers aur operations staff** bhi affected hain, kyunke failure notes mein un ka zikr hota hai. Ek summary "mausam ki wajah se der" ko "driver ki ghalti" bana sakti hai, ya kisi team ke liye zyada sakht zabaan use kar sakti hai.

**Fairness aur accuracy ka check:** attribution dispatch record se match kare, aur team alag alag reports ki zabaan compare kare.

**Disclosure:** pehle contract aur company ki requirements dekho. Agar woh khamosh hon, to ek routine operational report ke liye customer ko khaas notice shayad zaroori na ho. Employees par asar ka sawal alag se sochna chahiye.

## 5. Evidence (pehle quarter ke liye)

Control tab mazboot hai jab aap bata sakein ke woh kaam kar raha hai ya nahi.

```
Success measure      Account manager bhejne se pehle factual aur tone check poora kare.
Failure threshold    Koi bhi AI ki factual ghalti jo itni bari ho ke matter kare, customer tak pahunch jaye.
Monitor              Ayesha har mahine ek sample review kare.
Residual risk        Ek hi zabaan ka bias sab reports mein ho sakta hai aur har
                     report ki alag check mein bach jaye, isliye sample review
                     customers ke ARPAR bhi compare kare, sirf ek report ke andar nahi.
```

**Residual risk** ka matlab hai woh jo ab bhi ghalat ho sakta hai, jab saare planned controls kaam kar rahe hon.

## Ek zaroori baat

Ek chhota sa workflow, aur chaaron sawalon ne mil kar saat ठोस cheezein aur ek escalation point diye. Course kehta hai ke yeh **governance ko kaam ke design ka hissa** banata hai, baad mein jora hua kaagaz nahi.

## Workflow course se mel (meri observation)

Account manager ka gate workflow course ka **Collaborative step** hai: AI draft banata hai (delegate), named insaan check karta hai (gate).

Ek sawal aap se: is example mein Capability ke sawal ka jawab kya tha: **(a)** enable read-only, **(b)** escalate, ya **(c)** decline? Jawab likh dein, phir agla hissa lete hain: **Governance Record**, jo yeh sab ek page par likhta hai.

Ji, **bilkul sahi.** Jo workflow design karein, uske liye in 4 sawalon ke jawab **likhe hue** hone chahiye. Bas do cheezein add karni hain.

```
1. Case        Kya AI yeh kaam kar sakta hai? (aur gate: kaun, kya, kab)
2. Data        Kaunsa data jata hai, aur kya yeh raasta approved hai?
3. Capability  Kaunsa tool on kiya, aur woh kya kar sakta hai?
4. People      Kis par asar hoga, aur kya disclosure chahiye?
   + Evidence  Hum kaise jaanenge ke control kaam kar raha hai?
```

**Do tarmeemein:**

1. **Paanch hisse hain, chaar nahi.** Chaar sawal ke jawab, aur paanchwa **Evidence** (success measure, failure threshold, monitor, residual risk). Page par owner aur re-check ki wajahein (kab dobara dekhna hai) bhi hoti hain.
2. **Har kaam par nahi, sirf "meaningful work" par.** Jo kaam kisi aur ka data, kisi ka paisa, ya kisi insaan ke baare mein faisla chhute. Apni email ke lafz badalne ke liye page nahi bharte.

## Workflow design se jorna

```
Workflow design   --> har step ka owner (AI / Collaborative / Human)
Governance Record --> kya yeh kaam, data aur tool AI ke liye allowed hain,
                      aur kisi par unfair asar to nahi? Sab ek page par.
```

Dono saath chalte hain: map batata hai ke kaunsa step kis ko, aur record batata hai ke woh faisle kis wajah se aur kis ijazat se hue.

**Viva ke liye ek line:**

> Workflow design karte waqt Case, Data, Capability aur People ke jawab ek Governance Record par likhe hone chahiye, saath mein Evidence, taake koi bhi dekh sake ke kya tay hua aur kyun.
## Bilkul seedhi baat: kaam shuru karne se pehle 4 sawal ke jawab likh lo

Sochiye aap ek naya kaam AI ko dene wali hain: **customers ko har hafte ek report bhejna.** Shuru karne se pehle aap 4 sawalon ke jawab ek kaagaz par likhti hain. Bas itna hi.

```
1. Case        Kya yeh kaam AI ko de sakti hun?
               Jawab: AI draft banaye, account manager bhejne se pehle check kare.

2. Data        Kaunsa data AI ko jayega?
               Jawab: customer ke naam aur delivery ki tafseel (yellow),
               aur woh raasta approved hai.

3. Capability  AI ko kaunsa tool dena hai?
               Jawab: sirf parhne wala (read-only). Bhejna AI ka kaam nahi.

4. People      Kis par asar hoga?
               Jawab: customers aur drivers. Report mein unke baare mein
               jo likha jaye woh insaf se likha ho.
```

**Yeh jawab ek kaagaz par likhe honge, to koi bhi dekh sakta hai ke aap ne kya socha tha.** Is kaagaz ko **Governance Record** kehte hain.

## Ghar ki misaal

Aap ek helper ko ghar ka kaam dene se pehle likhti hain:

```
Kaun sa kaam?  Kaun si chabi?  Kis ko batana hai?  Masla ho to kise phone karna hai?
```

Phir koi poochhe to kaagaz dikha deti hain.

## Ek zaroori baat

Har chhote kaam ke liye nahi. Sirf woh kaam jis mein kisi aur ka data, kisi ka paisa, ya kisi insaan ke baare mein faisla ho.


## Section 7: Jab kuch ghalat ho jaye (incident ka pehla ghanta)

**Pehle masla:** governance ka matlab yeh nahi ke koi ghalti nahi hogi. Matlab yeh hai ke ghalti **jaldi saamne aaye**, taake roki ja sake.

**Ghar ki misaal (meri apni):** gas ki boo aaye to pehle gas band karte hain, phir bataate hain, phir dekhte hain kya hua. "Shayad theek ho jaye" kehna sab se mehenga parta hai.

## Ghalti ki paanch qisam (course ki)

```
Data       Info aise raaste se chali gayi jo us ke liye approved nahi tha.
Output     AI ka banaya hua kaam bahar gaya aur us mein bari ghalti ya nuqsan wali baat thi.
Action     AI tool ne woh bheja, badla, delete kiya, approve kiya ya share kiya jo nahi karna tha.
Security   Bahar ke content ne AI ko apni taraf mora (prompt injection).
Fairness   Chhantai ya ranking ne kuch logon ke saath na-insafi ki aur review ne nahi pakda.
```

## Pehle ghante ke 5 steps

```
1. PHAILNA ROKO       Aage forward, repost ya bekaar nayi copies mat banao.
2. FACTS LIKHO        Kya hua, kaunsa data, output ya action, kaunsa raasta, kab,
                      aur kya aage gaya ya nahi.
3. JALDI REPORT KARO  Apne organization ke incident raaste se. Sensitive ya regulated
                      cases mein waqt qanooni taur par bhi matter karta hai, to
                      "perfect wajah" ka intezar mat karo.
4. SAAF BAYAN DO      Andaza mat lagao, apna difa mat karo. Incident owner ko
                      bharosemand bayan chahiye.
5. HIDAYAT MAANO      Delete karna, notify karna, disclose karna, evidence bachana,
                      yeh sab incident owner tay karta hai. Aap akele nahi.
```

## Teen cheezein jo mat karo

```
- Chupke se delete kar do
- Intezar karo ke kuch na ho
- Dekho ke kisi ne notice kiya ya nahi
```

Kyun? Delete karne se **aap ki apni visibility** jati hai, data nahi, kyunke organization ya vendor ke records mein copy ab bhi ho sakti hai. Aur yeh investigation ya zaroori preservation mein rukawat daal sakta hai. Ghalti ko chhupana usay concealment bana deta hai.

Course ki line: **"the clock matters more than the polish."**

## Near miss bhi report karo

Near miss woh hai jahan ghalti hote hote bach gayi. Yeh bina poore incident ki qeemat ke dikhata hai ke process kahan uljha hua hai ya approved raasta kahan bahut mushkil hai.

## Managers ke liye ek baat

Pehli good-faith ghalti report karne wale ke saath company jaisa bartao karti hai, usi se tay hota hai ke agli das ghaltiyan report hongi ya chhupayi jayengi.

## Workflow course se mel (meri observation)

Workflow course ke Concept 17 ne kaha tha: stop, scope, tell, map. Us ka "pehle ghante ka poora procedure" isi Governance chapter mein hai (course ne khud yahan bheja tha). Dono ek doosre ke saath chalte hain: designer pehle se tay karta hai ke kaise rokna hai, aur incident ke waqt yeh 5 steps chalte hain.

## Ek sawal, sirf haan ya nahi

Aap ne galti se ek customer ki file ghalat raaste se upload kar di aur dar ke maare use chupke se delete kar diya aur kisi ko nahi bataya. Kya yeh sahi tareeqa hai?

Jawab dein, phir agle hissa mein **drift** (jab control khamoshi se kamzor hota hai) lete hain
