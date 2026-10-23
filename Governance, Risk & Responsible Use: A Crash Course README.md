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
