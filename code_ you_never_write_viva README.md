

````markdown
# Code You Never Write: Summary (Roman Urdu)

> 13 concepts, 4 parts, 1 kahani. Source: [Code You Never Write](https://agentfactory.panaversity.org/docs/code-you-never-write-crash-course)

![Code You Never Write - Big Picture](code-you-never-write-big-picture.svg)

## Fehrist

- [Kahani ki shuruaat](#kahani-ki-shuruaat-hum-yeh-kyun-parh-rahe-hain)
- [Part 1: Naya deal](#part-1-naya-deal)
- [Part 2: Code commission karna](#part-2-code-commission-karna-order-dena)
- [Part 3: Aik masla, paanch surfaces](#part-3-aik-masla-paanch-surfaces)
- [Part 4: Taqat, ehtiyaat ke saath](#part-4-taqat-ehtiyaat-ke-saath)
- [Projects aur unki definitions](#projects-aur-unki-definitions)
- [Phans jao to 6 fixes](#phans-jao-to-6-fixes)
- [Kahani ka nateeja](#kahani-ka-nateeja-viva-ke-liye)

---

## Kahani ki shuruaat: Hum yeh kyun parh rahe hain?

**Bookkeeper ki kahani:** Ek bookkeeper har mahine company ke kharchon ka record aur bank statement milati thi. Ek poori shaam line by line farq dhoondne mein lag jati thi. Phir usne AI se aam English mein kaha:

> "Yeh do files match honi chahiye; jo transaction aik mein hai aur doosri mein nahi, sab dhoondo."

Ek minute mein 23 mismatches aa gaye. Usne na code likha, na parha.

- **Course ka wada:** Aap masla batate hain. AI language chunta hai, code likhta hai, chalata hai aur theek karta hai. Aap kabhi code nahi likhte, aur uska syntax nahi parhte, lekin result check karna seekhte hain.
- **Syntax:** Code ki punctuation aur line by line grammar, jo seekhne mein mahine lagte hain.
- **Asal pehchaan:** Aap code ke **client** hain, contractor nahi. Achha client eentein nahi lagata; woh saaf brief deta hai, kaam ko naap kar check karta hai, aur jo banwaya woh sambhal kar rakhta hai.
- **Aazadi aur zimmedari:** Syntax na parhna aazadi hai. Result check karna zimmedari hai.
- **Prompting course se farq:** Wahan code ka khel wala hissa tha (game, web page). Yahan asli kaam hai, jahan grade, salary ya client ka paisa daaw par hai.

---

## Part 1: Naya deal

### Concept 1: Code ab coding ka mohtaaj nahi

Pehle do raaste the: programming seekho, ya kaam hath se karo, ya developer se **script** (dobara chalne wala chhota program jo file mein save ho) banwao aur do hafte intezar karo.

- **Naya deal:** AI developer hai, aap client. AI seconds mein, free mein, bina thake kaam karta hai.
- **Teen cheezein aik saath mature huin:**
  - AI chhote aur saaf bataye gaye masle ka chalta hua code likhta hai.
  - AI code khud chalata hai, **sandbox** mein: AI company ka aapki chat ke liye banaya hua temporary computer. Kuch tools aapki ijazat se aapki machine par bhi chalate hain.
  - Code toot jaye to error AI ke paas wapas jata hai aur AI khud theek karta hai.
- **2023 wali aadat bhoolein:** Tab AI code ka block de kar chala jata tha. Ab woh code likh kar usi reply mein chala bhi deta hai.
- **Naya sawal:** "Kya main yeh bana sakta hoon?" nahi, balki "Kya main isay bayan kar sakta hoon?" Agar aap bata sakte hain ke "done" kaisa dikhega, to aap code order kar sakte hain.
- **6 professions:** Bookkeeper, doctor (no-show rates), marketer, teacher, student (300 photos rename), network engineer (rozana health report).

### Concept 2: Code asal mein kya hai

Code exact instructions ki list hai jo computer bilkul theek, kisi bhi raftaar se, jitni baar chahein chalata hai.

- **Python:** Files, spreadsheets, data, charts aur reports ke liye. Aapko sab se zyada yahi nazar aayega, aur AI isay sab se achha jaanta hai kyunki training text mein Python sab se zyada hai.
- **JavaScript / TypeScript:** Jo cheez click karni ho: web tool, chhoti game, link se share hone wala calculator. **TypeScript** JavaScript hi hai, bas extra safety checks ke saath.
- **Language aap nahi chunte:** Yeh technical faisla hai, aur woh aap AI ko de rahe hain. Number chahiye to Python, button chahiye to JavaScript.
- **Code dekhna ijazat hai, zaroorat nahi:** Mechanic ka khula engine dikhata hai ke kaam ho raha hai, yeh nahi ke repair sahi hua.
- **Sab se zaroori property: Code is exact, in both directions.** Paisa aakhri paise tak sahi ginta hai, aur ghalat hukam bhi bilkul waise hi, bare paimane par poora karta hai. Taqat aur khatra aik hi property se aate hain.
- **Robot cook:** "20 minute" ki jagah "20 ghante" kaha gaya to khana koyla ban gaya. Robot fail nahi hua, **brief** fail hua.
- **Brief:** Kaam ki aam zubaan mein likhi hui tafseel jo aap AI ko dete hain. Achha brief bhi guarantee nahi, kyunki AI saaf brief ko bhi ghalat samajh sakta hai. Is liye result hamesha check karna hai.

### Concept 3: Dividing line, yani kaunsa masla code ka hai

Har prompt se pehle aik faisla: yeh AI ke **dimaagh** ka kaam hai ya uske **haathon** ka?

- **Answer problem:** AI apni reasoning se jawab de: draft, mashwara, summary, explanation.
- **Code problem:** AI ko aapke asli data par code likh kar chalana pade.

**VPRF, yani 4 signals (aik bhi ho to code problem):**

| Signal | Test | Misaal |
| --- | --- | --- |
| **Volume** | Itni cheezein jo hath se na ho sakein | 300 files, 5,000 rows |
| **Precision** | Aik ghalat digit ka nuqsan ho | Invoices, payroll, grades, paisa |
| **Repetition** | Agle mahine phir yahi kaam (sab se mazboot signal) | Month-end report |
| **Files** | Masla files mein hai, sentences mein nahi | Spreadsheets, logs, photos |

- **Trap:** "Roughly sales kaisi rahi?" baat cheet jaisa lagta hai, lekin agar faisla us number par hai to yeh code problem hai.
- **School fee example:** AI ne 8 families batayin jinki fees baaqi thi; asal mein 11 thin. AI ne skim kiya aur partial payment ko paid samjha. Ek line bacha sakti thi: "write and run code."

---

## Part 2: Code commission karna (order dena)

### Concept 4: AI ke haath hilwao, automatic vs explicit

AI khud decide karta hai ke code likhe ya nahi. Jo sawal nazar maar kar jawab dene layak lage, us par woh andaza laga deta hai. Andaza aur computation bilkul aik jaise dikhte hain, yahi **silent failure** hai.

**3 lines jo yaad karni hain:**

1. `"Write and run code to answer this."` Is se computation hoti hai.
2. `"Show me the code you ran."` Is se proof milta hai: code block nahi to code nahi chala.
3. `"Before analyzing anything, tell me the exact row count, the column names, and the date range."` Yeh sab se sasta lie detector hai. Andaza ho to round number aur ghalat column names aate hain.

- **"Code" likhein, "Python" nahi.** Language AI ko chunne dein.
- **Shak ho to poochhein:** "Are you running code or estimating? If estimating, stop and run code."
- **Ulta bhi sach:** Essay persuasive hai ya nahi, iske liye code mat maangein.
- **The tell:** Data ke baare mein aisa jawab jis mein code block, row count ya "yeh calculate kiya" na ho, woh analysis nahi, sirf raaye hai.

### Concept 5: Program nahi, masla brief karo

Achhe brief mein koi technical lafz nahi hota (loops, libraries, language). Aap bas batate hain ke achha nateeja kaisa dikhta hai. Thoda programming jaanne wale aksar bure brief likhte hain, kyunki woh "kaise" par zyada aur "kya" par kam zor dete hain.

**Brief ke 5 hisse:**

1. **Goal:** Kaam ho jaye to kaunsa masla hal hoga?
2. **Input:** Kaunsi files, kis format mein, kitni rows.
3. **Output:** Kya wapas chahiye (number, table, chart, saaf file, HTML report).
4. **Rules:** Woh limits jo ajnabi ko pata na hon (school year August mein shuru hota hai, "Pending" ka matlab abhi jama nahi hua).
5. **Edge cases:** Kharab data ke liye pehle se faisle (khali rows, duplicates, ghalat date format).

```markdown
# Brief: [kaam ka naam]
## Goal
## Input
## Output
## Rules
## Edge cases
```

- **Markdown spec:** Yeh brief Markdown headings mein likha jata hai. Har heading aik cheez kam karti hai jo AI ko guess karni padti.
- **Rules mein aapka professional ilm hota hai.** Har ghalat analysis kisi aise rule tak jata hai jo aap jaante the lekin likha nahi.
- **Edge case ki standard line:** "Jo row parh na sako, guess mat karo; skip karo aur aakhir mein list do." Is se chhupi ghalti nazar aane wali report ban jati hai.
- **CSV:** Spreadsheet jo comma se alag kiye saade rows ki shakal mein save hoti hai.
- **Apne edge cases nahi pata? Poochh lein:** "Pehle files dekho aur batao kya unclear, inconsistent ya ajeeb hai."
- **Tarteeb yaad rakhein:** Inspect → Ask → Brief.

### Concept 6: Jo kaam parh nahi sakte, usay verify karna

Model ke paas apna truth-checker nahi hota, lekin code ke saath aapke paas aik checker hai: aap usay chala sakte hain. Expert ko uske nateejon se check karte hain, jaise accountant ko apne records ke totals se.

**5 checks (asaan se mushkil):**

1. **Known-answer test:** Code ko aise chhote hisse par chalayein jiska jawab aap jaante hain (March ka total, aik student ka grade). Yeh sab se taqatwar check hai.
2. **Reality questions:** 1,400 rows andar gayin aur 1,381 report mein hain, to 19 kahan gayin? Sab se bara customer wahi hai jo aap jaante hain?
3. **Plain-English replay:** AI se kahein code ne kya kiya woh aam English mein step by step batao. Zyada tar asal ghaltiyan procedure ki hoti hain, typing ki nahi.
4. **Adversarial pass:** AI apne hi kaam par hamla kare: assumptions, sab se kamzor kari, har claim ko 1–10 confidence.
5. **Cross-model check:** Wohi brief aur data doosri company ke AI ko dein. **Limit:** Jo rule brief mein likha hi nahi, us mein dono aik saath ghalti kar ke agree kar sakte hain.

**Stakes ke hisaab se:**

- **Apni curiosity:** Reality questions.
- **Colleague ka kaam:** Known-answer + replay.
- **Paisa, grades, health ya signed kaam:** Paanchon checks, aur insaan important claims review kare.

**Misaalein aur definitions:**

- **Pharmacist:** Usne data mein jaan boojh kar 10 units ka fake gap daala. Code ne fake gap aur 4 asli gaps pakre. Fake pakra gaya, is liye asli par yaqeen aaya.
- **Uncle Bob (Robert C. Martin, "Clean Code" ke author):** July 2026 mein usne kaha ke woh ab apne agents ka code nahi parhta, balki usay "extreme constraints" yani automatic checks ki layers mein rakhta hai. Tarteeb yaad rakhein: **pehle checks banaye, phir code parhna chhoda.** Uska bharosa feeling nahi, checks ka size hai.
- **Test:** Chhota extra program jo main code ko check kar ke pass ya fail bataye.
- **Mutation testing:** Main code ko jaan boojh kar thoda thoda torna aur dekhna ke koi test pakarta hai ya nahi. Jo test chup rahe, woh kuch sabit nahi karta. Pharmacist ne bina naam jaane yahi kiya.

> **Kabhi skip na hone wala rule:** Precision wale number par tab tak amal na karein jab tak usay kam az kam aik aise jawab se test na kar liya ho jo aap khud jaante hain. **Known-answer test aapki firewall hai.**

### Concept 7: Error baat cheet hai, nakami nahi

Error project ka fail hona nahi; computer bilkul theek bata raha hai ke usay kya chahiye.

- **Laal error aaye aur script ruk jaye:** Poora error paste karein aur kahein `"Diagnose it, fix the code, and run it again."` Aapko error samajhne ki zaroorat nahi, sirf aage bhejna hai.
- **Surface:** Woh jagah jahan AI code chala sakta hai (browser chat, ya aapke computer ka tool).
- **Wrong-but-running:** Koi error nahi, lekin number ghalat lage. "Ghalat hai, theek karo" mat kahein. Doctor ko symptom batane ki tarah kahein:
  > "Total 4.2 million aaya, lekin mujhe pata hai 12 million ke qareeb tha. Row count, date range aur pehli 5 rows dikhao."

  Aksar wajah fauran mil jati hai: sirf pehli sheet parhi, "1,200" ko text samjha, ya export adhoora tha.
- **Same fix 3 dafa fail:** Khodna band karein. Kahein: "Step back, masla naye sire se bayan karo, aur do bilkul alag approaches do." Teen strikes ka matlab approach ghalat hai. Chat lambi aur confused ho to brief ke saath nayi chat shuru karein.
- **Marketer aur "codec" error:** Usne bina samjhe error paste kiya; 40 second mein file encoding theek ho gayi. Error parhna zaroori nahi, paste karne ki himmat zaroori hai.

### Concept 8: Script rakh lo, hal kiya hua masla button ban jata hai

Repetition signal ka faida yeh hai ke aik dafa likhi script hamesha aapki hai.

**3 aadatein:**

1. **Script file maangein:** Clear naam, aur upar aam English mein likha ho ke script kya karti hai, kaunsi files chahiye aur kaunse rules lagati hai.
2. **Brief script ke saath rakhein:** Script "kaise" hai machines ke liye. Brief "kya aur kyun" hai insaano aur aage ke AI sessions ke liye. Isay **Intent Layer** kehte hain: files mein likhe aapke iraade, itne exact ke AI un par amal kar sake.
3. **Aik folder mein ghar:** `my-scripts/` ke andar har kaam ka subfolder, jis mein brief, script aur aik chhoti sample input file ho. Yeh sample kal ka known-answer test hai.

```text
my-scripts/
  essay-submissions/
    brief.md          <- kya aur kyun, aapke lafzon mein
    submissions.py    <- code (aap phir bhi nahi parhte)
    sample-class/     <- inputs jinka sahi jawab aap jaante hain
```

- **Script ke saath vs bina:** Har mahine dobara samjhane ki zaroorat nahi, mahine ba mahine rules mein farq (drift) nahi aata, aur colleague ko folder de dein to woh minuton mein kaam shuru kar deta hai.
- **Clinic manager:** March mein script banayi; August tak Friday ko 30 second ka kaam. Nayi branch ko folder de diya. **"Describe once, run forever, hand to anyone."**
- **Chat mein scripts paida hoti hain, aapki machine par rehti hain.**

---

## Part 3: Aik masla, paanch surfaces

Ab tak ki saari skills har jagah aik jaisi hain. Sirf yeh badalta hai ke code kahan chalta hai aur kya chhoo sakta hai.

- **5 surfaces, 3 jagahen:**
  - **Browser sandbox:** Claude.ai, ChatGPT, Gemini
  - **Terminal:** Claude Code, OpenCode
  - **Desktop app:** Cowork, OpenWork
- **Running job:** 12 mahine ki expense CSV files merge karna, category ke hisaab se total, duplicates flag karna, aur chart ke saath HTML report banana.

### Concept 9: Claude.ai, home surface

Code Anthropic ki taraf sandbox mein chalta hai, aur aapke computer ko kuch nahi hota. Isi liye seekhne ke liye yeh zero-risk jagah hai.

- **Taqat:** Kuch install nahi karna, koi risk nahi, aik dafa ke kaam ke liye perfect, aur brief → code → verify → iterate poora nazar aata hai.
- **Limit:**
  - Sandbox sirf upload ki hui files dekhta hai, yani 40 files ke liye 40 uploads, aur network devices mein login yahan se mumkin nahi.
  - Sandbox temporary hai; script download na ki to chat ke saath khatam.
  - Har dafa ke kaam mein dobara upload karna padta hai.

> "Chat sandbox aik workshop hai jahan aap jaate hain, aapki files wahan nahi rehtin."

### Concept 10: Claude Code aur OpenCode, aapke folder mein agent

Dono **terminal** mein chalte hain (saadi text window jahan computer ko commands likhi jati hain).

- **Tasawwur:** Tool install ho to terminal aik chat box ban jata hai jo folder ke andar baitha hai. Naye laptop ka khali terminal chat box nahi hota; woh sirf computer commands samajhta hai.
- **Agent:** AI jo kai steps ka kaam khud karta hai aur aapki files par kaam kar sakta hai. Files pehle se wahan hain, upload ki zaroorat nahi. Scripts folder mein hamesha rehti hain, aur errors khud theek hote hain.
- **Kab:** Jab code aapki machine par, schedule par chalana ho, ya aise systems chhoone hon jahan browser nahi pohanchta. Misaal: network engineer jis ke 40 devices ki report subah khud ban jati hai.
- **Claude Code vs OpenCode:** Claude Code polished hai aur Claude chalata hai. OpenCode mein model khud chun sakte hain, free aur self-hosted bhi.
- **Non-programmers bhi yahan ke hain:** Is ke liye apni files aur apna masla jaanna kaafi hai, code nahi. Kai heavy users accountants aur researchers hain jo upload kar kar ke thak gaye the.

### Concept 11: Cowork aur OpenWork, safety ritual ke saath delegation

Desktop apps jin mein terminal jitni file power hai, lekin aam app window mein, knowledge workers ke liye. Andar se yeh aksar code likh kar hi kaam karti hain.

- **Plan-then-approve:** App plan likh kar ruk jati hai. Aap aam English mein plan parhte hain, ghalat assumption pakarte hain, phir approve karte hain. Yeh Concept 6 ka plain-English replay hai, bas kaam se **pehle**.

**Kaunsi surface kab:**

| Aapki situation | Kya use karein |
| --- | --- |
| Aik dafa ka sawal, kuch files | Claude.ai |
| Seekhna ya kisi aur ka computer | Claude.ai |
| Masla aapke folders mein hai aur dobara aayega | Claude Code / OpenCode |
| Wahi, lekin app aur pehle plan chahiye | Cowork / OpenWork |
| Schedule par ya doosre systems tak | Claude Code / OpenCode |

- **Graduation signal:** Jab upload karna aapke hafte ka sab se pareshan kun kaam ban jaye, tab aage barhein.

---

## Part 4: Taqat, ehtiyaat ke saath

### Concept 12: Blast radius

Claude.ai par ghaltiyan free hain. Code aapki machine par chale to "exact in both directions" asli khatra ban jata hai. Agent ki delete ki hui files aksar recycle bin mein nahi jatin, aur script ne edit ki hui file ki undo history nahi hoti.

- **Blast radius:** Run ghalat ho jaye to sab se bura kya ho sakta hai.

**4 rules:**

1. **Copies pehle:** Folder ki backup copy banayein. Script kai dafa saaf chal jaye to us script ke liye yeh rule dheela kar sakte hain.
2. **Dry run:** Har change ki list pehle dekhein (purana naam aur naya naam) aur approve karein. Cowork mein yeh built-in hai; terminal mein har dafa khud maangna padta hai.
3. **Sab se chhota folder:** Home directory (aapki saari personal files wala top folder), "Documents" ya poori disk kabhi nahi.
4. **Output nayi files mein:** Originals kabhi overwrite na hon. Ghalti ho to nayi file delete kar dein.

**3 sentence wala standard prompt:**

```text
Copy the folder to a backup first. Show me your plan of operations before
changing anything, and wait for approval. Write all output to new files.
Never modify the originals.
```

- **Permission ladder:** Pehle thodi azadi, phir zyada. Bharosa khaas scripts par hota hai jinka record achha ho, technology par nahi.
- **Researcher:** Dry run mein 40 deletions dikhin, jin mein 6 ghalat thin (alag interviews jinki length aur naam milte the). Rule ko "content match karo, naam aur size nahi" mein badla aur 34 sahi deletions approve kiye.

### Concept 13: Map ka kinara, yani aik prompt ke code ki hadd

- **Hadd ke andar:** Har reconciliation, rollup, rename, merge, clean, cross-check, chart aur report jo VPRF ka koi signal fire kare. Zyada tar professionals ke liye saal ke saikron ghante.
- **Hadd ke bahar (aik prompt ka code kaafi nahi):**
  - **Software jis mein log login karein:** Accounts, payments, aik saath kai users, raat 3 baje bhi chalne wali service. Yeh products hain, scripts nahi.
  - **Hamesha chalne wali automation jiske asli nateeje hon:** Jaise "har hafte clients ko khud email bhejo". Yeh tab chalti hai jab koi dekh nahi raha, jahan Concept 6 ke checks nahi pohanchte. Jo worker khud chale woh **Digital FTE** hai: AI worker jo poora role sambhale, employee ki tarah.
  - **Undo na hone wale high-stakes kaam:** Tax filing submit karna, mass email bhejna, trade lagana. Code tayyar kare, insaan khud bheje.
  - **Computation ke libaas mein judgment:** "Compute karo kis employee ko promote karein." Hisaab aasaan hai; criteria hi asal masla hain, aur woh aapke hain.

> **"Code computes. You decide."**

---

## Projects aur unki definitions

- **Catch:** Aik sacchi baat jo AI ke code ne dhoondi, aap pehle se nahi jaante the, aur jis par aap kuch kar sakte hain. Jaise cancel karne wali subscription, dispute karne wala charge, ya dost se wapas lene wala paisa.
- **Off-the-shelf-app test:** Kya kisi company ne isi kaam ki app pehle se banayi hai (jaise bill split ke liye Splitwise)? Agar haan, to yeh yahan ke liye ghalat masla hai, kyunki app tab hi banti hai jab rules sab ke liye aik jaise hon.
- **Market of one:** Sahi masla ulta hota hai: aapke rules, aapka data ka gand, aur aisa jawab jo sirf aap confirm kar sakte hain.

**4 projects aur unke known answers:**

1. **Money Detective:** Purani history mein paisa kahan ja raha hai. Total income 23,000 aur PrimeVideo 199 × 4 = 796 aana chahiye. Catch: bhooli hui subscription, 8 July ka double Foodpanda charge, aur asal leak food delivery (lagbhag 4,050).
2. **What's My Grade, Really:** Teacher ke grading rules. Do sab se kam homework (45, 60) hata kar average 88.75 aana chahiye.
3. **The Books Don't Match:** Do records ka farq. 8 log × 500 = 4,000 hone chahiye; hisaab 500 kam nikla (Usman ka 300 pizza ka tha, aur aik 500 kis ka hai pata nahi).
4. **Photo Gallery Rescue:** Duplicates safely delete karna. Code **perceptual hash** (har image ka chhota fingerprint) se compare karta hai. Delete se pehle backup aur list zaroori, kyunki do alag sunsets bhi match ho sakte hain.

---

## Phans jao to 6 fixes

1. **File nahi khul rahi:** AI se poochhein file mein kya masla hai; aksar dobara export karna padta hai.
2. **Code block nazar nahi aaya:** "Stop. Write and run code, show the code, row count first."
3. **Number match nahi karta:** Symptom batayein: AI ka number, aapka number, row count, aur pehli 5 rows.
4. **Wohi fix baar baar fail:** 3 strikes ke baad 2 bilkul alag approaches maangein.
5. **Private data ka dar:** Pehle names aur account numbers hata kar cleaned copy banwayein, aur tool ki data policy check karein.
6. **Free limit khatam:** Reset ka intezar karein, ya wohi brief kisi doosri model family mein paste karein.

> **Pattern:** Jab phans jayein, to AI ko bata dein ke kahan phanse hain.

---

## Kahani ka nateeja (viva ke liye)

**Aik pehchaan aur aik skill:** Aap client hain, contractor nahi. Aur aap aise kaam par bharosa kar sakte hain jo aap dekh nahi sakte, kyunki aapne usay kisi aisi cheez se test kiya jo aap pehle se jaante the.

### Yaad rakhne ki chain

1. Bayan kar sakte ho? (Concept 1)
2. Code exact hai, dono taraf (Concept 2)
3. VPRF se pehchano (Concept 3)
4. "Write and run code" bolo (Concept 4)
5. 5-part brief do (Concept 5)
6. Known answer se check karo (Concept 6)
7. Error paste karo (Concept 7)
8. Script rakh lo (Concept 8)
9. Sandbox mein seekho (Concept 9)
10. Folder mein agent (Concept 10)
11. Plan approve karo (Concept 11)
12. 4 safety rules (Concept 12)
13. Hadd pehchano (Concept 13)

### Pichhle lesson se link

AI Prompting ka Concept 10 kehta hai "code chalwao". Yeh course us ka poora version hai:

- **Kab chalwana hai:** VPRF
- **Kaise order karna hai:** Brief
- **Kaise check karna hai:** Known answer
- **Kaise safe rehna hai:** Blast radius
````

**Image ke liye:** README mein image ki line tabhi chalegi jab `code-you-never-write-big-picture.svg` bhi repo ke usi folder mein upload ho. Image upload nahi karni to file mein upar wali `![...](...)` line delete kar dein.

Ab har Concept ka naam wahi English title hai jo lesson mein likha hai, aur uske neeche Roman Urdu matlab italic mein hai. Parts ke naam bhi English mein kar diye hain. Neeche poora text aik box mein hai; copy button daba kar GitHub par paste kar dein.

````markdown
# Code You Never Write: Summary (Roman Urdu)

> 13 concepts, 4 parts, 1 kahani. Source: [Code You Never Write](https://agentfactory.panaversity.org/docs/code-you-never-write-crash-course)

![Code You Never Write - Big Picture](code-you-never-write-big-picture.svg)

## Fehrist

- [Kahani ki shuruaat](#kahani-ki-shuruaat-hum-yeh-kyun-parh-rahe-hain)
- [Part 1: The deal](#part-1-the-deal)
- [Part 2: Commissioning code](#part-2-commissioning-code)
- [Part 3: One problem, five surfaces](#part-3-one-problem-five-surfaces)
- [Part 4: Power, safely held](#part-4-power-safely-held)
- [Projects aur unki definitions](#projects-aur-unki-definitions)
- [Phans jao to 6 fixes](#phans-jao-to-6-fixes)
- [Kahani ka nateeja](#kahani-ka-nateeja-viva-ke-liye)

---

## Kahani ki shuruaat: Hum yeh kyun parh rahe hain?

**Bookkeeper ki kahani:** Ek bookkeeper har mahine company ke kharchon ka record aur bank statement milati thi. Ek poori shaam line by line farq dhoondne mein lag jati thi. Phir usne AI se aam English mein kaha:

> "Yeh do files match honi chahiye; jo transaction aik mein hai aur doosri mein nahi, sab dhoondo."

Ek minute mein 23 mismatches aa gaye. Usne na code likha, na parha.

- **Course ka wada:** Aap masla batate hain. AI language chunta hai, code likhta hai, chalata hai aur theek karta hai. Aap kabhi code nahi likhte, aur uska syntax nahi parhte, lekin result check karna seekhte hain.
- **Syntax:** Code ki punctuation aur line by line grammar, jo seekhne mein mahine lagte hain.
- **Asal pehchaan:** Aap code ke **client** hain, contractor nahi. Achha client eentein nahi lagata; woh saaf brief deta hai, kaam ko naap kar check karta hai, aur jo banwaya woh sambhal kar rakhta hai.
- **Aazadi aur zimmedari:** Syntax na parhna aazadi hai. Result check karna zimmedari hai.
- **Prompting course se farq:** Wahan code ka khel wala hissa tha (game, web page). Yahan asli kaam hai, jahan grade, salary ya client ka paisa daaw par hai.

---

## Part 1: The deal

*Naya deal*

### Concept 1: Code is no longer gated by coding

*Code ab coding ka mohtaaj nahi*

Pehle do raaste the: programming seekho, ya kaam hath se karo, ya developer se **script** (dobara chalne wala chhota program jo file mein save ho) banwao aur do hafte intezar karo.

- **Naya deal:** AI developer hai, aap client. AI seconds mein, free mein, bina thake kaam karta hai.
- **Teen cheezein aik saath mature huin:**
  - AI chhote aur saaf bataye gaye masle ka chalta hua code likhta hai.
  - AI code khud chalata hai, **sandbox** mein: AI company ka aapki chat ke liye banaya hua temporary computer. Kuch tools aapki ijazat se aapki machine par bhi chalate hain.
  - Code toot jaye to error AI ke paas wapas jata hai aur AI khud theek karta hai.
- **2023 wali aadat bhoolein:** Tab AI code ka block de kar chala jata tha. Ab woh code likh kar usi reply mein chala bhi deta hai.
- **Naya sawal:** "Kya main yeh bana sakta hoon?" nahi, balki "Kya main isay bayan kar sakta hoon?" Agar aap bata sakte hain ke "done" kaisa dikhega, to aap code order kar sakte hain.
- **6 professions:** Bookkeeper, doctor (no-show rates), marketer, teacher, student (300 photos rename), network engineer (rozana health report).

### Concept 2: What code actually is (the 60-second version)

*Code asal mein kya hai*

Code exact instructions ki list hai jo computer bilkul theek, kisi bhi raftaar se, jitni baar chahein chalata hai.

- **Python:** Files, spreadsheets, data, charts aur reports ke liye. Aapko sab se zyada yahi nazar aayega, aur AI isay sab se achha jaanta hai kyunki training text mein Python sab se zyada hai.
- **JavaScript / TypeScript:** Jo cheez click karni ho: web tool, chhoti game, link se share hone wala calculator. **TypeScript** JavaScript hi hai, bas extra safety checks ke saath.
- **Language aap nahi chunte:** Yeh technical faisla hai, aur woh aap AI ko de rahe hain. Number chahiye to Python, button chahiye to JavaScript.
- **Code dekhna ijazat hai, zaroorat nahi:** Mechanic ka khula engine dikhata hai ke kaam ho raha hai, yeh nahi ke repair sahi hua.
- **Sab se zaroori property: Code is exact, in both directions.** Paisa aakhri paise tak sahi ginta hai, aur ghalat hukam bhi bilkul waise hi, bare paimane par poora karta hai. Taqat aur khatra aik hi property se aate hain.
- **Robot cook:** "20 minute" ki jagah "20 ghante" kaha gaya to khana koyla ban gaya. Robot fail nahi hua, **brief** fail hua.
- **Brief:** Kaam ki aam zubaan mein likhi hui tafseel jo aap AI ko dete hain. Achha brief bhi guarantee nahi, kyunki AI saaf brief ko bhi ghalat samajh sakta hai. Is liye result hamesha check karna hai.

### Concept 3: The dividing line: which problems are code problems

*Kaunsa masla code ka hai*

Har prompt se pehle aik faisla: yeh AI ke **dimaagh** ka kaam hai ya uske **haathon** ka?

- **Answer problem:** AI apni reasoning se jawab de: draft, mashwara, summary, explanation.
- **Code problem:** AI ko aapke asli data par code likh kar chalana pade.

**VPRF, yani 4 signals (aik bhi ho to code problem):**

| Signal | Test | Misaal |
| --- | --- | --- |
| **Volume** | Itni cheezein jo hath se na ho sakein | 300 files, 5,000 rows |
| **Precision** | Aik ghalat digit ka nuqsan ho | Invoices, payroll, grades, paisa |
| **Repetition** | Agle mahine phir yahi kaam (sab se mazboot signal) | Month-end report |
| **Files** | Masla files mein hai, sentences mein nahi | Spreadsheets, logs, photos |

- **Trap:** "Roughly sales kaisi rahi?" baat cheet jaisa lagta hai, lekin agar faisla us number par hai to yeh code problem hai.
- **School fee example:** AI ne 8 families batayin jinki fees baaqi thi; asal mein 11 thin. AI ne skim kiya aur partial payment ko paid samjha. Ek line bacha sakti thi: "write and run code."

---

## Part 2: Commissioning code

*Code commission karna, yani order dena*

### Concept 4: Make the AI's hands move: automatic vs. explicit

*AI ke haath hilwao*

AI khud decide karta hai ke code likhe ya nahi. Jo sawal nazar maar kar jawab dene layak lage, us par woh andaza laga deta hai. Andaza aur computation bilkul aik jaise dikhte hain, yahi **silent failure** hai.

**3 lines jo yaad karni hain:**

1. `"Write and run code to answer this."` Is se computation hoti hai.
2. `"Show me the code you ran."` Is se proof milta hai: code block nahi to code nahi chala.
3. `"Before analyzing anything, tell me the exact row count, the column names, and the date range."` Yeh sab se sasta lie detector hai. Andaza ho to round number aur ghalat column names aate hain.

- **"Code" likhein, "Python" nahi.** Language AI ko chunne dein.
- **Shak ho to poochhein:** "Are you running code or estimating? If estimating, stop and run code."
- **Ulta bhi sach:** Essay persuasive hai ya nahi, iske liye code mat maangein.
- **The tell:** Data ke baare mein aisa jawab jis mein code block, row count ya "yeh calculate kiya" na ho, woh analysis nahi, sirf raaye hai.

### Concept 5: Brief the problem, not the program

*Program nahi, masla brief karo*

Achhe brief mein koi technical lafz nahi hota (loops, libraries, language). Aap bas batate hain ke achha nateeja kaisa dikhta hai. Thoda programming jaanne wale aksar bure brief likhte hain, kyunki woh "kaise" par zyada aur "kya" par kam zor dete hain.

**Brief ke 5 hisse:**

1. **Goal:** Kaam ho jaye to kaunsa masla hal hoga?
2. **Input:** Kaunsi files, kis format mein, kitni rows.
3. **Output:** Kya wapas chahiye (number, table, chart, saaf file, HTML report).
4. **Rules:** Woh limits jo ajnabi ko pata na hon (school year August mein shuru hota hai, "Pending" ka matlab abhi jama nahi hua).
5. **Edge cases:** Kharab data ke liye pehle se faisle (khali rows, duplicates, ghalat date format).

```markdown
# Brief: [kaam ka naam]
## Goal
## Input
## Output
## Rules
## Edge cases
```

- **Markdown spec:** Yeh brief Markdown headings mein likha jata hai. Har heading aik cheez kam karti hai jo AI ko guess karni padti.
- **Rules mein aapka professional ilm hota hai.** Har ghalat analysis kisi aise rule tak jata hai jo aap jaante the lekin likha nahi.
- **Edge case ki standard line:** "Jo row parh na sako, guess mat karo; skip karo aur aakhir mein list do." Is se chhupi ghalti nazar aane wali report ban jati hai.
- **CSV:** Spreadsheet jo comma se alag kiye saade rows ki shakal mein save hoti hai.
- **Apne edge cases nahi pata? Poochh lein:** "Pehle files dekho aur batao kya unclear, inconsistent ya ajeeb hai."
- **Tarteeb yaad rakhein:** Inspect → Ask → Brief.

### Concept 6: Verifying work you cannot read

*Jo kaam parh nahi sakte, usay verify karna*

Model ke paas apna truth-checker nahi hota, lekin code ke saath aapke paas aik checker hai: aap usay chala sakte hain. Expert ko uske nateejon se check karte hain, jaise accountant ko apne records ke totals se.

**5 checks (asaan se mushkil):**

1. **Known-answer test:** Code ko aise chhote hisse par chalayein jiska jawab aap jaante hain (March ka total, aik student ka grade). Yeh sab se taqatwar check hai.
2. **Reality questions:** 1,400 rows andar gayin aur 1,381 report mein hain, to 19 kahan gayin? Sab se bara customer wahi hai jo aap jaante hain?
3. **Plain-English replay:** AI se kahein code ne kya kiya woh aam English mein step by step batao. Zyada tar asal ghaltiyan procedure ki hoti hain, typing ki nahi.
4. **Adversarial pass:** AI apne hi kaam par hamla kare: assumptions, sab se kamzor kari, har claim ko 1–10 confidence.
5. **Cross-model check:** Wohi brief aur data doosri company ke AI ko dein. **Limit:** Jo rule brief mein likha hi nahi, us mein dono aik saath ghalti kar ke agree kar sakte hain.

**Stakes ke hisaab se:**

- **Apni curiosity:** Reality questions.
- **Colleague ka kaam:** Known-answer + replay.
- **Paisa, grades, health ya signed kaam:** Paanchon checks, aur insaan important claims review kare.

**Misaalein aur definitions:**

- **Pharmacist:** Usne data mein jaan boojh kar 10 units ka fake gap daala. Code ne fake gap aur 4 asli gaps pakre. Fake pakra gaya, is liye asli par yaqeen aaya.
- **Uncle Bob (Robert C. Martin, "Clean Code" ke author):** July 2026 mein usne kaha ke woh ab apne agents ka code nahi parhta, balki usay "extreme constraints" yani automatic checks ki layers mein rakhta hai. Tarteeb yaad rakhein: **pehle checks banaye, phir code parhna chhoda.** Uska bharosa feeling nahi, checks ka size hai.
- **Test:** Chhota extra program jo main code ko check kar ke pass ya fail bataye.
- **Mutation testing:** Main code ko jaan boojh kar thoda thoda torna aur dekhna ke koi test pakarta hai ya nahi. Jo test chup rahe, woh kuch sabit nahi karta. Pharmacist ne bina naam jaane yahi kiya.

> **Kabhi skip na hone wala rule:** Precision wale number par tab tak amal na karein jab tak usay kam az kam aik aise jawab se test na kar liya ho jo aap khud jaante hain. **Known-answer test aapki firewall hai.**

### Concept 7: When it breaks: errors are dialogue, not failure

*Error baat cheet hai, nakami nahi*

Error project ka fail hona nahi; computer bilkul theek bata raha hai ke usay kya chahiye.

- **Laal error aaye aur script ruk jaye:** Poora error paste karein aur kahein `"Diagnose it, fix the code, and run it again."` Aapko error samajhne ki zaroorat nahi, sirf aage bhejna hai.
- **Surface:** Woh jagah jahan AI code chala sakta hai (browser chat, ya aapke computer ka tool).
- **Wrong-but-running:** Koi error nahi, lekin number ghalat lage. "Ghalat hai, theek karo" mat kahein. Doctor ko symptom batane ki tarah kahein:
  > "Total 4.2 million aaya, lekin mujhe pata hai 12 million ke qareeb tha. Row count, date range aur pehli 5 rows dikhao."

  Aksar wajah fauran mil jati hai: sirf pehli sheet parhi, "1,200" ko text samjha, ya export adhoora tha.
- **Same fix 3 dafa fail:** Khodna band karein. Kahein: "Step back, masla naye sire se bayan karo, aur do bilkul alag approaches do." Teen strikes ka matlab approach ghalat hai. Chat lambi aur confused ho to brief ke saath nayi chat shuru karein.
- **Marketer aur "codec" error:** Usne bina samjhe error paste kiya; 40 second mein file encoding theek ho gayi. Error parhna zaroori nahi, paste karne ki himmat zaroori hai.

### Concept 8: Keep the script: a solved problem becomes a button

*Script rakh lo, hal kiya hua masla button ban jata hai*

Repetition signal ka faida yeh hai ke aik dafa likhi script hamesha aapki hai.

**3 aadatein:**

1. **Script file maangein:** Clear naam, aur upar aam English mein likha ho ke script kya karti hai, kaunsi files chahiye aur kaunse rules lagati hai.
2. **Brief script ke saath rakhein:** Script "kaise" hai machines ke liye. Brief "kya aur kyun" hai insaano aur aage ke AI sessions ke liye. Isay **Intent Layer** kehte hain: files mein likhe aapke iraade, itne exact ke AI un par amal kar sake.
3. **Aik folder mein ghar:** `my-scripts/` ke andar har kaam ka subfolder, jis mein brief, script aur aik chhoti sample input file ho. Yeh sample kal ka known-answer test hai.

```text
my-scripts/
  essay-submissions/
    brief.md          <- kya aur kyun, aapke lafzon mein
    submissions.py    <- code (aap phir bhi nahi parhte)
    sample-class/     <- inputs jinka sahi jawab aap jaante hain
```

- **Script ke saath vs bina:** Har mahine dobara samjhane ki zaroorat nahi, mahine ba mahine rules mein farq (drift) nahi aata, aur colleague ko folder de dein to woh minuton mein kaam shuru kar deta hai.
- **Clinic manager:** March mein script banayi; August tak Friday ko 30 second ka kaam. Nayi branch ko folder de diya. **"Describe once, run forever, hand to anyone."**
- **Chat mein scripts paida hoti hain, aapki machine par rehti hain.**

---

## Part 3: One problem, five surfaces

*Aik masla, paanch surfaces*

Ab tak ki saari skills har jagah aik jaisi hain. Sirf yeh badalta hai ke code kahan chalta hai aur kya chhoo sakta hai.

- **5 surfaces, 3 jagahen:**
  - **Browser sandbox:** Claude.ai, ChatGPT, Gemini
  - **Terminal:** Claude Code, OpenCode
  - **Desktop app:** Cowork, OpenWork
- **Running job:** 12 mahine ki expense CSV files merge karna, category ke hisaab se total, duplicates flag karna, aur chart ke saath HTML report banana.

### Concept 9: Claude.ai: the home surface (and ChatGPT, Gemini)

*Seekhne ki ghar wali jagah*

Code Anthropic ki taraf sandbox mein chalta hai, aur aapke computer ko kuch nahi hota. Isi liye seekhne ke liye yeh zero-risk jagah hai.

- **Taqat:** Kuch install nahi karna, koi risk nahi, aik dafa ke kaam ke liye perfect, aur brief → code → verify → iterate poora nazar aata hai.
- **Limit:**
  - Sandbox sirf upload ki hui files dekhta hai, yani 40 files ke liye 40 uploads, aur network devices mein login yahan se mumkin nahi.
  - Sandbox temporary hai; script download na ki to chat ke saath khatam.
  - Har dafa ke kaam mein dobara upload karna padta hai.

> "Chat sandbox aik workshop hai jahan aap jaate hain, aapki files wahan nahi rehtin."

### Concept 10: Claude Code & OpenCode: the agent in your folder

*Aapke folder mein agent*

Dono **terminal** mein chalte hain (saadi text window jahan computer ko commands likhi jati hain).

- **Tasawwur:** Tool install ho to terminal aik chat box ban jata hai jo folder ke andar baitha hai. Naye laptop ka khali terminal chat box nahi hota; woh sirf computer commands samajhta hai.
- **Agent:** AI jo kai steps ka kaam khud karta hai aur aapki files par kaam kar sakta hai. Files pehle se wahan hain, upload ki zaroorat nahi. Scripts folder mein hamesha rehti hain, aur errors khud theek hote hain.
- **Kab:** Jab code aapki machine par, schedule par chalana ho, ya aise systems chhoone hon jahan browser nahi pohanchta. Misaal: network engineer jis ke 40 devices ki report subah khud ban jati hai.
- **Claude Code vs OpenCode:** Claude Code polished hai aur Claude chalata hai. OpenCode mein model khud chun sakte hain, free aur self-hosted bhi.
- **Non-programmers bhi yahan ke hain:** Is ke liye apni files aur apna masla jaanna kaafi hai, code nahi. Kai heavy users accountants aur researchers hain jo upload kar kar ke thak gaye the.

### Concept 11: Cowork & OpenWork: delegation with a safety ritual

*Safety ritual ke saath kaam saunpna*

Desktop apps jin mein terminal jitni file power hai, lekin aam app window mein, knowledge workers ke liye. Andar se yeh aksar code likh kar hi kaam karti hain.

- **Plan-then-approve:** App plan likh kar ruk jati hai. Aap aam English mein plan parhte hain, ghalat assumption pakarte hain, phir approve karte hain. Yeh Concept 6 ka plain-English replay hai, bas kaam se **pehle**.

**Kaunsi surface kab:**

| Aapki situation | Kya use karein |
| --- | --- |
| Aik dafa ka sawal, kuch files | Claude.ai |
| Seekhna ya kisi aur ka computer | Claude.ai |
| Masla aapke folders mein hai aur dobara aayega | Claude Code / OpenCode |
| Wahi, lekin app aur pehle plan chahiye | Cowork / OpenWork |
| Schedule par ya doosre systems tak | Claude Code / OpenCode |

- **Graduation signal:** Jab upload karna aapke hafte ka sab se pareshan kun kaam ban jaye, tab aage barhein.

---

## Part 4: Power, safely held

*Taqat, ehtiyaat ke saath*

### Concept 12: Blast radius: the rules for code that touches your files

*Files chhoone wale code ke rules*

Claude.ai par ghaltiyan free hain. Code aapki machine par chale to "exact in both directions" asli khatra ban jata hai. Agent ki delete ki hui files aksar recycle bin mein nahi jatin, aur script ne edit ki hui file ki undo history nahi hoti.

- **Blast radius:** Run ghalat ho jaye to sab se bura kya ho sakta hai.

**4 rules:**

1. **Copies pehle:** Folder ki backup copy banayein. Script kai dafa saaf chal jaye to us script ke liye yeh rule dheela kar sakte hain.
2. **Dry run:** Har change ki list pehle dekhein (purana naam aur naya naam) aur approve karein. Cowork mein yeh built-in hai; terminal mein har dafa khud maangna padta hai.
3. **Sab se chhota folder:** Home directory (aapki saari personal files wala top folder), "Documents" ya poori disk kabhi nahi.
4. **Output nayi files mein:** Originals kabhi overwrite na hon. Ghalti ho to nayi file delete kar dein.

**3 sentence wala standard prompt:**

```text
Copy the folder to a backup first. Show me your plan of operations before
changing anything, and wait for approval. Write all output to new files.
Never modify the originals.
```

- **Permission ladder:** Pehle thodi azadi, phir zyada. Bharosa khaas scripts par hota hai jinka record achha ho, technology par nahi.
- **Researcher:** Dry run mein 40 deletions dikhin, jin mein 6 ghalat thin (alag interviews jinki length aur naam milte the). Rule ko "content match karo, naam aur size nahi" mein badla aur 34 sahi deletions approve kiye.

### Concept 13: The edge of the map, and what's across it

*Map ka kinara, yani aik prompt ke code ki hadd*

- **Hadd ke andar:** Har reconciliation, rollup, rename, merge, clean, cross-check, chart aur report jo VPRF ka koi signal fire kare. Zyada tar professionals ke liye saal ke saikron ghante.
- **Hadd ke bahar (aik prompt ka code kaafi nahi):**
  - **Software jis mein log login karein:** Accounts, payments, aik saath kai users, raat 3 baje bhi chalne wali service. Yeh products hain, scripts nahi.
  - **Hamesha chalne wali automation jiske asli nateeje hon:** Jaise "har hafte clients ko khud email bhejo". Yeh tab chalti hai jab koi dekh nahi raha, jahan Concept 6 ke checks nahi pohanchte. Jo worker khud chale woh **Digital FTE** hai: AI worker jo poora role sambhale, employee ki tarah.
  - **Undo na hone wale high-stakes kaam:** Tax filing submit karna, mass email bhejna, trade lagana. Code tayyar kare, insaan khud bheje.
  - **Computation ke libaas mein judgment:** "Compute karo kis employee ko promote karein." Hisaab aasaan hai; criteria hi asal masla hain, aur woh aapke hain.

> **"Code computes. You decide."**

---

## Projects aur unki definitions

- **Catch:** Aik sacchi baat jo AI ke code ne dhoondi, aap pehle se nahi jaante the, aur jis par aap kuch kar sakte hain. Jaise cancel karne wali subscription, dispute karne wala charge, ya dost se wapas lene wala paisa.
- **Off-the-shelf-app test:** Kya kisi company ne isi kaam ki app pehle se banayi hai (jaise bill split ke liye Splitwise)? Agar haan, to yeh yahan ke liye ghalat masla hai, kyunki app tab hi banti hai jab rules sab ke liye aik jaise hon.
- **Market of one:** Sahi masla ulta hota hai: aapke rules, aapka data ka gand, aur aisa jawab jo sirf aap confirm kar sakte hain.

**4 projects aur unke known answers:**

1. **Money Detective:** Purani history mein paisa kahan ja raha hai. Total income 23,000 aur PrimeVideo 199 × 4 = 796 aana chahiye. Catch: bhooli hui subscription, 8 July ka double Foodpanda charge, aur asal leak food delivery (lagbhag 4,050).
2. **What's My Grade, Really:** Teacher ke grading rules. Do sab se kam homework (45, 60) hata kar average 88.75 aana chahiye.
3. **The Books Don't Match:** Do records ka farq. 8 log × 500 = 4,000 hone chahiye; hisaab 500 kam nikla (Usman ka 300 pizza ka tha, aur aik 500 kis ka hai pata nahi).
4. **Photo Gallery Rescue:** Duplicates safely delete karna. Code **perceptual hash** (har image ka chhota fingerprint) se compare karta hai. Delete se pehle backup aur list zaroori, kyunki do alag sunsets bhi match ho sakte hain.

---

## Phans jao to 6 fixes

1. **File nahi khul rahi:** AI se poochhein file mein kya masla hai; aksar dobara export karna padta hai.
2. **Code block nazar nahi aaya:** "Stop. Write and run code, show the code, row count first."
3. **Number match nahi karta:** Symptom batayein: AI ka number, aapka number, row count, aur pehli 5 rows.
4. **Wohi fix baar baar fail:** 3 strikes ke baad 2 bilkul alag approaches maangein.
5. **Private data ka dar:** Pehle names aur account numbers hata kar cleaned copy banwayein, aur tool ki data policy check karein.
6. **Free limit khatam:** Reset ka intezar karein, ya wohi brief kisi doosri model family mein paste karein.

> **Pattern:** Jab phans jayein, to AI ko bata dein ke kahan phanse hain.

---

## Kahani ka nateeja (viva ke liye)

**Aik pehchaan aur aik skill:** Aap client hain, contractor nahi. Aur aap aise kaam par bharosa kar sakte hain jo aap dekh nahi sakte, kyunki aapne usay kisi aisi cheez se test kiya jo aap pehle se jaante the.

### Yaad rakhne ki chain

1. **Code is no longer gated by coding:** Bayan kar sakte ho?
2. **What code actually is:** Code exact hai, dono taraf
3. **The dividing line:** VPRF se pehchano
4. **Make the AI's hands move:** "Write and run code" bolo
5. **Brief the problem, not the program:** 5-part brief do
6. **Verifying work you cannot read:** Known answer se check karo
7. **Errors are dialogue:** Error paste karo
8. **Keep the script:** Script rakh lo
9. **Claude.ai, the home surface:** Sandbox mein seekho
10. **Claude Code & OpenCode:** Folder mein agent
11. **Cowork & OpenWork:** Plan approve karo
12. **Blast radius:** 4 safety rules
13. **The edge of the map:** Hadd pehchano

### Pichhle lesson se link

AI Prompting ka Concept 10 kehta hai "code chalwao". Yeh course us ka poora version hai:

- **Kab chalwana hai:** VPRF
- **Kaise order karna hai:** Brief
- **Kaise check karna hai:** Known answer
- **Kaise safe rehna hai:** Blast radius
````

<img width="1600" height="2260" alt="download" src="https://github.com/user-attachments/assets/45b59adb-dad2-4748-83b5-a5df7a549b2d" />


**Q1. Commissioning code kya hai?**
Course ka Part 2. Matlab code ka "order dena". Is mein 5 kaam aate hain: AI se computation karwana (Concept 4), brief likhna (5), result verify karna (6), errors handle karna (7), script keep karna (8).

**Q2. Answer problem kya hai aur code problem kya hai?**
Answer problem woh hai jiska jawab AI apni reasoning se de sake (drafting, advice, summary, explain). Code problem woh hai jahan AI ko aapke real data par code likh kar run karna parta hai. Misaal: "polite email likho" answer problem hai, "2,000 rows ka total nikalo" code problem.

**Q3. VPRF kya hai?**
Code problem ke 4 signals: Volume, Precision, Repetition, Files. Koi ek bhi fire kare to woh code problem hai. Agar ek bhi fire na ho to answer problem hai.

**Q4. Sandbox kya hai?**
AI company ki taraf ka temporary computer jahan aapka code chalta hai. Aapki apni machine ko kuch nahi hota, isliye Claude.ai zero-risk surface hai.

**Q5. Brief kya hai?**
Job ki plain-English description jo aap AI ko dete hain. Is mein koi technical lafz nahi hota (loops, libraries, language ka naam nahi). Course ka usool: "Brief the problem, not the program."

**Q6. Rules aur Edge cases kya hain?**
Rules woh limits hain jo ek stranger ko nahi pata hoti (jaise "Pending" ka matlab aapke system mein "abhi submit nahi hua"). Edge cases woh faisle hain ke kharab data par kya karna hai, pehle se tay (blank row, duplicate, ghalat date format). Rules mein aapka professional knowledge hota hai.

**Q7. Known-answer test kya hai?**
Code ko ek aise chhote hisse par chalana jiska jawab aap pehle se jaanti hain. Agar code wohi jawab de to baaqi par bharosa "earned" hota hai, sirf umeed nahi.

**Q8. Reality questions kya hain?**
Woh sawal jo aap output se apne knowledge ke hisaab se poochti hain. Jaise: rows in vs rows out (1,400 gaye aur 1,381 aaye, 19 kahan gaye?), ya "biggest customer wohi hai jo main jaanti hoon?"

**Q9. Plain-English replay kya hai?**
AI se kehna ke apna code colleague ko samjhane ke andaz mein saada lafzon mein bayan kare (blank rows aur duplicates ka kya kiya). Zyadatar real errors procedure ki hoti hain, aur ghalat procedure English mein bhi ghalat parhi jati hai.

**Q10. Adversarial pass kya hai?**
AI se kehna ke apne hi kaam ko ghalat sabit karne ki koshish kare: kaunsi assumptions hain, weakest link kaunsi hai, har claim ko 1 se 10 confidence do aur wajah batao.

**Q11. Cross-model check kya hai?**
Wohi brief aur data ek doosre company ke AI mein chalana aur numbers milana. High-stakes results ke liye hai.

**Q12. Wrong-but-running kya hai?**
Koi error message nahi aata, lekin number us se alag hota hai jo aap jaanti hain. Misaal: report 4.2 million dikhati hai jabke aap jaanti hain ke 12 million hona chahiye.

**Q13. Intent Layer kya hai?**
Aapki likhi hui intentions, files mein rakhi hui, itni exact ke AI un par amal kar sake. Brief isi ka hissa hai.

**Q14. Surface, terminal aur agent kya hain?**
Surface woh jagah hai jahan AI aapka code chala sakta hai (browser chat, terminal, desktop app). Terminal ek plain text window hai jahan aap computer ko instructions type karti hain. Agent woh AI hai jo multi-step kaam karta hai aur aapki files par act kar sakta hai.

**Q15. Plan-then-approve kya hai?**
Cowork aur OpenWork ka feature: app pehle plain English mein plan likhta hai aur aapki approval ka intezar karta hai, tab kaam karta hai. Yeh plain-English replay hai jo kaam se **pehle** ho jata hai.

**Q16. Blast radius kya hai?**
Agar run ghalat chala jaye to sab se bura nuqsan kya ho sakta hai. 4 safety rules isi ko chhota karte hain.

**Q17. Dry run kya hai?**
Un sab changes ki list jo code karne wala hai, kuch bhi karne se pehle. Ghalat-fehmi tab pakri jati hai jab woh lafzon mein ho, actions mein nahi.

**Q18. Digital FTE kya hai?**
Aisa AI worker jo poora role carry kare, employee ki tarah. Course ke Concept 13 mein bataya hai ke yeh is course se aage ka topic hai (jaise "har hafte clients ko khud email bhejna").

**Q19. Market of one aur off-the-shelf-app test kya hai?**
Project ka masla chunne ka filter. Pehle pucho: "Kya iske liye pehle se koi app hai?" Agar haan (jaise Splitwise), to galat problem hai kyunke app tab bante hain jab rules sab ke liye same hon. Market of one woh problem hai jiske rules sirf aapke hain.

**Q20. Discovery prompt kya hai?**
Jab aapko apne data ke edge cases nahi pata, to pehle AI se kaho: "Kuch karne se pehle files examine karo aur batao kya unclear, inconsistent ya surprising hai." Phir us ke jawab se Edge cases likho. Order: inspect, ask, then brief.

# Section B: "Kitni types, kitne options?"

**Q21. Course ke kitne concepts aur kitne parts hain?**
13 concepts, 4 parts:
1. The deal (Concepts 1 se 3)
2. Commissioning code (4 se 8)
3. Five surfaces (9 se 11)
4. Power, safely held (12 aur 13)

**Q22. VPRF ke kitne signals hain?**
4 signals: Volume (zyada items), Precision (ghalat digit ka nuqsan), Repetition (baar baar karna), Files (masla files mein hai). Koi ek kaafi hai.

**Q23. Brief ke kitne sections hain?**
5 sections: Goal, Input, Output, Rules, Edge cases. Beginners aksar Rules aur Edge cases skip kar dete hain.

**Q24. Concept 4 ki "pin above your desk" lines kitni hain?**
3 lines:
1. "Write and run code to answer this."
2. "Show me the code you ran."
3. "Pehle exact row count, column names aur date range batao."

**Q25. Verification ladder mein kitne steps hain, aur order kya hai?**
5 steps, effort ke hisaab se badhte hue:
1. Known-answer test
2. Reality questions
3. Plain-English replay
4. Adversarial pass
5. Cross-model check

Course kehta hai pehle 3 zyadatar situations cover karte hain.

**Q26. Stakes ke hisaab se kitni verification chahiye?**
3 levels:
- Personal curiosity (apna kharcha): Reality questions
- Colleague ka bharose wala kaam: Known-answer test + Plain-English replay
- Paisa, grades, health, signed cheezein: saare 5 + insaan review

**Q27. Errors ke kitne patterns hain?**
3 patterns:
1. Red text, script ruki: poora error paste karo, "diagnose, fix, rerun."
2. Chalti hai magar number contradict karta hai: symptom aur expected value batao, row count aur sample rows dikhane ko kaho.
3. Wohi fix 3 baar fail: step back, problem naye sire se, 2 completely different approaches maango.

**Q28. Keep the script ki habit ke kitne hisse hain?**
3 hisse:
1. Script ko file ke taur par maango, top par plain-English note ke saath.
2. Brief script ke saath rakho.
3. Dono ko ek folder mein rakho (brief.md, script, aur ek sample input jo known-answer test banega).

**Q29. Kitne surfaces hain aur kitni qism ki jagah?**
5 surfaces, 3 qism ki jagah:
- Browser sandbox: Claude.ai (aur ChatGPT, Gemini)
- Terminal in your folder: Claude Code aur OpenCode
- Desktop app: Cowork aur OpenWork

**Q30. Safety rules kitne hain?**
4 rules:
1. Work on copies
2. See changes before they happen (dry run)
3. Point the agent at the smallest folder
4. Write output to new files, never over the originals

**Q31. Concept 13 mein kitne kaam "edge of the map" ke paar hain?**
4 qism:
1. Software jis mein doosre log login karte hain
2. Always-on automation jiske real consequences hon
3. High-stakes acts jinka undo nahi (tax filing, mass email, trade)
4. Judgment jo computation ke libaas mein ho

**Q32. Code ki kitni languages ke naam yaad rakhne hain?**
2 naam: Python (numbers, files, reports) aur JavaScript/TypeScript (jo click karna ho). Aap language kabhi nahi chunti, output ke hisaab se AI chunta hai.

**Q33. 2023 se ab tak AI ne kitni cheezein seekhi hain?**
3 cheezein: code **likhta** hai, **run** karta hai, aur **repair** karta hai.

**Q34. Course ke kitne projects hain aur unke naam?**
4 projects:
1. Money Detective
2. What's My Grade, Really
3. The Books Don't Match
4. Photo Gallery Rescue

**Q35. Project "done" kab hota hai? (Money Detective)**
3 shartein: code woh 2 numbers reproduce kare jo aap pehle se jaanti thin (total in 23,000 aur PrimeVideo 796), aap ko kam az kam ek sachi cheez mile jo aap nahi jaanti thin aur is hafte amal kar sakein, aur ek saved script ho jo agle mahine dobara chale.

**Q36. Stuck hone par kitne common symptoms diye hain?**
6 symptoms:
1. File open nahi hoti
2. Code block nahi aaya
3. Number match nahi karta
4. Same fix baar baar fail
5. Private data upload ka dar
6. Free-tier limit khatam

**Q37. "By the end, you'll be able to" mein kitni skills hain?**
6 skills: code problem spot karna, 5-section brief likhna, computation force karna, unreadable result check karna, scripts safely run karna, aur jo banaya usay keep karna.

# Section C: "Kyun?"

**Q38. Prompt mein "write and run code" kyun kehna parta hai?**
Kyunke AI aap ke prompt ki awaaz se decide karta hai ke code likhe ya estimate kare. Estimate aur computation dono ek jaise confident lagte hain, aur screen par koi nishani nahi hoti. Isliye Precision wale kaam mein faisla AI par nahi chhorna.

**Q39. "In Python" kyun nahi likhte?**
Language chunna ek technical judgment hai jo aap AI ko de chuki hain. "In Python" kehne se aap use ghalat guess par majboor kar sakti hain, aur aap ko pata bhi nahi chalega.

**Q40. Rules section itna important kyun hai?**
Kyunke har ghalat analysis kisi aise rule se aati hai jo aap jaanti thin magar likha nahi. Misaal: school administrator ne AI ko kaha "kaun se families payment mein peeche hain", AI ne 8 bataye jabke asal 11 the, kyunke "partial payment ko paid maan liya". Rule hona chahiye tha: "koi bhi unpaid balance wala family behind hai."

**Q41. Known-answer test sab se powerful kyun hai?**
Kyunke code exact hota hai, ghalat mein bhi. Aap code parh nahi sakti, lekin aap woh jawab jaanti hain jo AI nahi jaanta. Agar code aapke jaanay hue jawab tak pahunche to bharosa earned hai.

**Q42. Code ko parhe bina kaise bharosa karein? (core answer of Concept 6)**
Jaise aap accountant ko check karti hain: uska qanoon dobara nahi parhti, balke apne records se total milati hain. Aap results ko apne independent knowledge se verify karti hain.

**Q43. Uncle Bob ka example kyun diya hai?**
Yeh dikhane ke liye ke code na parhna beginner ka compromise nahi. Clean Code ke musannif ne bhi agents ka code parhna chhoda, lekin pehle "extreme constraints" (checks) banaye. Sabaq: checks pehle, parhna chhodna baad mein.

**Q44. Error aaye to AI ko paste kyun karte hain, khud samajhne ki koshish kyun nahi?**
Kyunke error computer ki taraf se "mujhe yeh chahiye" ka precise bayan hai, aur AI usay parh kar khud theek kar leta hai. Marketer ka "codec" error 40 second mein theek hua. Course kehta hai: "Reading errors is not required. Willingness to paste them is."

**Q45. Script ko keep kyun karte hain?**
Kyunke ek baar describe karo to hamesha chalti hai. Rules script mein frozen ho jate hain to May aur June ki logic same rehti hai, aur folder kisi colleague ko dene se woh minutes mein productive ho jata hai.

**Q46. Claude.ai se shuru kyun karte hain?**
Kyunke sandbox mein galtiyan free hain, aap ki machine ko kuch nahi hota. Agle surface par tab jao jab uploading hafte ka annoying hissa ban jaye.

**Q47. Backup kyun zaroori hai (Rule 1)?**
Kyunke agent se delete ki hui files aksar recycle bin skip karti hain, aur script se edit ki hui files ki koi undo history nahi hoti.

**Q48. Dry run kyun karte hain?**
Researcher ne agent se duplicate recordings hatane ko kaha. Dry run ki list mein 40 deletions thin, jinme 6 ghalat nikliin (alag interviews, same length). Rule theek karke 34 sahi delete hui. Dry run ne 6 interviews bachayin.

**Q49. Output nayi file mein kyun (Rule 4)?**
Taake originals saaf rahein aur har run undo ho sake (nayi file delete kar do). Isay har brief ke Output section mein standing line bana lo.

**Q50. Smallest folder kyun (Rule 3)?**
Confused script `expenses-2025/` mein 12 CSVs kharab kar sakti hai (jinki backup hai). Lekin drive ke top par confused ho to aapki zindagi kharab kar sakti hai.

**Q51. Cross-model check ki limit kya hai aur kyun?**
Dono AI ne wohi brief parha. Agar aap ne koi rule likha hi nahi, to dono ek hi ghalti kar sakte hain aur agree bhi karenge.

**Q52. Judgment ko code ko kyun nahi dete (Concept 13)?**
"Kaun promote ho" ka arithmetic aasan hai, lekin criteria hi asal masla hai aur woh aapke hain. Course ka jumla: "Code computes. You decide."

# Section D: Farq wale sawal

**Q53. Answer problem aur code problem mein farq?**
Answer problem: AI mind se jawab deta hai (draft, advice, summary). Code problem: AI hands se kaam karta hai (total, merge, rename, reconcile, chart). Agar koi ek VPRF signal fire kare to code problem.

**Q54. Python aur JavaScript mein farq?**
Python: number, file, report. JavaScript/TypeScript: jo cheez click ya browser mein khole (calculator, quiz, dashboard).

**Q55. Backup aur dry run mein farq?**
Backup (Rule 1): ghalti ke **baad** wapas lene ke liye. Dry run (Rule 2): ghalti hone se **pehle** list dekhne ke liye. Dono saath lagte hain.

**Q56. Red-text error aur wrong-but-running mein farq?**
Red text mein script ruk jati hai, aap poora error paste karti hain. Wrong-but-running mein koi error nahi, bas number galat hai, aur "it's wrong, fix it" nahi kehte, balke symptom aur expected value batate hain aur AI se row count aur sample rows dikhane ko kehte hain.

**Q57. Rules aur Edge cases mein farq?**
Rules: aapka domain knowledge (jo stranger nahi jaanta). Edge cases: imperfect data par kya karna hai (skip karo aur list do).

**Q58. Known-answer test aur reality questions mein farq?**
Known-answer test: ek chhote hisse par code chalao jiska jawab aap jaanti hain. Reality questions: poore output ko apne knowledge se pucho (rows in vs out, biggest customer kaun hai).

**Q59. Plain-English replay aur adversarial pass mein farq?**
Replay: AI batata hai ke code ne **kya kiya** (procedure). Adversarial pass: AI batata hai ke **kahan ghalat ho sakta hai** (weak points aur confidence scores).

**Q60. Known-answer test aur cross-model check mein farq?**
Known-answer test aap ke apne knowledge par based hai. Cross-model check doosre AI ki agreement par. Cross-model ki limit hai ke dono ek hi brief ki ghalti share kar sakte hain.

**Q61. Brief aur script mein farq?**
Script = **how** (machine ke liye). Brief = **what aur why** (insaan aur future AI ke liye). Dono saath rakhne se baad mein "rule badal gaya" kehna kaafi hota hai.

**Q62. Claude.ai aur Claude Code mein farq?**
Claude.ai: sandbox, files upload karni parti hain, script chat ke saath khatam (jab tak download na karein). Claude Code: aapke folder ke andar, files pehle se saamne, scripts rehti hain, errors khud theek karta hai, schedule par chal sakta hai.

**Q63. Claude Code aur Cowork mein farq?**
Dono aapki files par kaam karte hain. Claude Code terminal mein hai, aur dry run aapko khud maangna parta hai. Cowork desktop app hai jo plan-then-approve by design deta hai.

**Q64. Claude Code aur OpenCode mein farq?**
Experience same hai (chat box in a folder). Claude Code Anthropic ka hai aur Claude chalata hai. OpenCode open-source hai aur aap model chun sakti hain, free aur self-hosted bhi.

**Q65. Sandbox aur aapki machine mein farq?**
Sandbox: temporary, AI company ki taraf, sirf uploaded files dekhta hai, risk zero. Aapki machine: files wahin hain, scripts permanent hain, magar galti real files ko chhoo sakti hai (isliye 4 safety rules).

**Q66. Script aur Digital FTE mein farq?**
Script ek kaam ka chhota button hai jo aap chalati hain. Digital FTE poora role carry karta hai aur khud chalta hai, aksar nigrani ke baghair. Isliye woh Concept 6 ke checks ki hadd se bahar hai.

# Section E: Scenario sawal

**Q67. School administrator ne spreadsheet AI ko di aur poocha "kaun se families peeche hain". AI ne 8 batae, asal 11 the. Kya hua aur kya fix?**
AI ne **answer** kiya jab **compute** karna tha, skim kar ke partial payment ko paid maan liya. Fix: "write and run code to find them" kehna, aur Rules mein likhna ke "koi bhi unpaid balance wala family behind hai."

**Q68. 1,400 rows andar gayin, report mein 1,381 hain. Kaun sa check?**
Reality questions. Pucho: baaqi 19 kahan gayin?

**Q69. Wohi fix teen baar fail ho gaya. Kya karein?**
Step back, problem naye sire se likho, aur 2 bilkul alag approaches maango. Teen strikes ka matlab approach galat hai, typing nahi. Agar chat bohat lambi aur ulajh gayi ho to naya chat shuru karo brief aur jo seekha uske saath.

**Q70. Report ne 4.2 million sales dikhayi, aap jaanti hain 12 million thi. Kya karein?**
Yeh wrong-but-running hai. Symptom aur expected value batao aur AI se row count, date range aur pehli 5 rows jaisi code ne dekhi dikhane ko kaho. Aam wajahein: Excel ki sirf pehli sheet padhi gayi, "1,200" ko text samjha, ya export aadha band ho gaya.

**Q71. Agent ne duplicates delete karne ka plan bheja, 40 files hain. Kya karein?**
Dry run list parho. Agar kuch aisi files hain jo asal mein duplicate nahi (jaise researcher ki 6 interviews), rule theek karo (name aur size ki jagah content par match karo), dobara list lo, phir approve karo. Pehle backup zaroor ho.

**Q72. Pharmacist ne dispensing log aur stock counts ka cross-check script se karwana tha. Usne kya kiya?**
Data ki copy mein ek jaali gap (10 units) dali. Script ne woh bhi pakdi aur 4 asli bhi. Yeh known-answer test ka sab se elegant roop hai, mutation testing jaisa idea.

**Q73. Teacher har Monday teen exports ko ek report mein merge karti hai. Kaun sa signal?**
Repetition, sab se strong signal. Isse script ek asset ban jati hai, "run my script on this week's files."

**Q74. Koi polite email likhna chahta hai. Code problem hai?**
Nahi. Koi VPRF signal fire nahi hota (no volume, precision, repetition, files). Pure answer problem hai.

**Q75. "Roughly kaisi trend rahi sales?" aur us number par budget ka faisla hai. Kya karein?**
Yeh VPRF ki trap hai: sawal casual lagta hai magar Precision fire karta hai. Code problem hai, "write and run code" kaho.

**Q76. Ek hi reply mein AI ne analysis di lekin koi code block, row count ya "maine compute kiya" nahi. Kya samjhein?**
The tell: yeh data ke baare mein opinion hai, analysis nahi. Kaho: "Stop. Write and run code, show me the code, aur pehle row count do."

**Q77. 40 files baar baar upload karna annoying ho gaya. Kya karein?**
Yeh graduation signal hai. Claude Code ya OpenCode par jao jo folder ke andar kaam karta hai. Agar app chahiye aur kaam se pehle plan dekhna hai to Cowork ya OpenWork.

**Q78. Aap chahti hain AI har hafte clients ko khud email bheje.**
Edge of the map ke paar: unattended automation jahan Concept 6 ke checks ki pahunch nahi. Isay Digital FTE jaisa worker chahiye. Course kehta hai: code **prepare** kare, insaan **send** kare.

**Q79. "Kaun employees promote hon" ka AI se hisaab karwana hai.**
Judgment wearing a computation costume. Arithmetic aasan hai magar criteria asal masla hain aur woh aapke hain. Code computes, you decide.

**Q80. Books Don't Match project mein 500 ka ek payment unknown number se aaya. AI kya kare?**
Guess nahi karna. Rules mein likha tha: "no name I recognize, flag it." Result: 4,000 ke muqable mein 500 short, Usman ka sirf pizza wala 300 (dues nahi), aur ek mystery 500. Deliverable: group chat ka ek jumla jo aap aaj raat bhej sakein.

**Q81. Bookkeeper ki kahani (course ka opening). Kya hua?**
Do files (apna spending record aur bank statement) har mahine match nahi hoti thin. Usne English mein likha "find every transaction that is in one but not the other." Aik minute mein 23 mismatches mil gaye, har ek ki amount aur date ke saath. Usne kabhi code nahi parha.

**Q82. Messy calories file mein "650 kcal", "1,100" aur duplicate row thi. Kaise tamed hui?**
Rules aur Edge cases se: "kcal ya comma ko plain number maano", "bilkul same row do baar ho to ek baar ginte hain", "date khali ho to skip karke list do." In dono sections ko hata do to mess wapas aa jati hai.

# Section F: Rapid-fire (ek line mein jawab)

- Commissioning code? Code ka order dena (Concepts 4 se 8).
- Code problem? Jahan AI ko real data par code likh kar run karna ho.
- VPRF? Volume, Precision, Repetition, Files.
- Strongest signal? Repetition.
- Brief ke 5 sections? Goal, Input, Output, Rules, Edge cases.
- Rules? Woh limits jo stranger ko nahi pata.
- Edge cases? Kharab data par pehle se tay faisla.
- Discovery prompt? Pehle data examine karwana, phir brief likhna.
- Concept 4 ki teesri line? Row count, column names, date range pehle.
- Known-answer test? Jis hisse ka jawab aap jaanti hain us par code chalao.
- Reality questions? Rows in vs rows out jaise sawal.
- Plain-English replay? AI saade lafzon mein bataye code ne kya kiya.
- Adversarial pass? AI apna kaam khud todne ki koshish kare.
- Cross-model check? Wohi brief doosre AI mein chalao.
- Wrong-but-running? Error nahi, magar number ghalat.
- Three strikes? Approach badlo, typing nahi.
- Intent Layer? Aapki likhi hui intentions files mein.
- Sandbox? AI company ka temporary computer.
- Terminal reframe? Folder ke andar baitha chat box.
- Plan-then-approve? Pehle plan, phir approval, phir kaam.
- Blast radius? Ghalti ka sab se bura nuqsan.
- Dry run? Kuch karne se pehle changes ki list.
- 4 safety rules? Copy, dry run, smallest folder, new files (C-D-C-N).
- Digital FTE? AI worker jo poora role carry kare.
- Market of one? Aise rules jo sirf aap ke hain.
- Sab se bara usool? You are the client, not the contractor. Trust work you cannot see because you tested it against something you already knew.
<svg xmlns="http://www.w3.org/2000/svg" width="1600" height="2260" viewBox="0 0 1600 2260">
  <style>
    text { font-family: "Segoe UI", Arial, sans-serif; fill: #1d2433; }
    .title { font-size: 46px; font-weight: 700; }
    .sub { font-size: 22px; fill: #5b6475; }
    .h { font-size: 27px; font-weight: 700; }
    .n { font-size: 19px; font-weight: 700; fill: #ffffff; text-anchor: middle; }
    .t { font-size: 24px; font-weight: 700; }
    .l { font-size: 19px; }
    .y { font-size: 18px; font-weight: 600; fill: #b45309; }
    .w { fill: #ffffff; }
    .bh { font-size: 25px; font-weight: 700; }
    .bl { font-size: 18px; }
  </style>

  <rect width="1600" height="2260" fill="#f6f7fb"/>

  <!-- Title -->
  <text x="800" y="72" class="title" text-anchor="middle">Code You Never Write — Big Picture</text>
  <text x="800" y="112" class="sub" text-anchor="middle">13 concepts · 4 parts · Aap code ke CLIENT ho, contractor nahi</text>

  <!-- Foundation -->
  <rect x="40" y="140" width="1520" height="122" rx="18" fill="#1d2433"/>
  <text x="70" y="182" class="w" font-size="18" letter-spacing="2" opacity="0.75">PEHCHAAN</text>
  <text x="70" y="222" class="w" font-size="28" font-weight="700">Aap CLIENT ho</text>
  <text x="70" y="250" class="w" font-size="18" opacity="0.85">Likhna nahi: brief do, check karo, rakh lo</text>
  <rect x="560" y="158" width="980" height="86" rx="14" fill="#374151" stroke="#9ca3af" stroke-dasharray="7 5"/>
  <text x="1050" y="196" class="w" font-size="27" font-weight="700" text-anchor="middle">“Code is exact, in both directions.”</text>
  <text x="1050" y="228" class="w" font-size="19" text-anchor="middle" opacity="0.85">Sahi hukam bhi perfect, ghalat hukam bhi perfect. Is liye har result check karo.</text>

  <!-- Chain -->
  <text x="800" y="296" text-anchor="middle" font-size="20" font-weight="600" fill="#5b6475">Bayan karo → VPRF → “Run code” bolo → Brief → Known answer → Error paste → Script rakho → Surface → Safety → Hadd</text>

  <!-- ================= PART 1 ================= -->
  <rect x="40" y="315" width="745" height="910" rx="18" fill="#eef4ff" stroke="#2563eb" stroke-width="3"/>
  <text x="62" y="360" class="h" fill="#2563eb">PART 1 · Naya deal</text>

  <g transform="translate(55,385)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#2563eb"/>
    <circle cx="40" cy="36" r="18" fill="#2563eb"/><text x="40" y="43" class="n">1</text>
    <text x="68" y="44" class="t">Code ab coding ka mohtaaj nahi</text>
    <text x="28" y="80" class="l">AI likhta + chalata (sandbox) + khud theek karta hai</text>
    <text x="28" y="107" class="l">Script = dobara chalne wala program · AI developer, aap client</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: “Bana sakta hoon?” nahi, “Bayan kar sakta hoon?”</text>
  </g>

  <g transform="translate(55,552)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#2563eb"/>
    <circle cx="40" cy="36" r="18" fill="#2563eb"/><text x="40" y="43" class="n">2</text>
    <text x="68" y="44" class="t">Code kya hai (60-second version)</text>
    <text x="28" y="80" class="l">Python = data, files, reports · JS/TS = click wali cheez</text>
    <text x="28" y="107" class="l">Language aap nahi chunte · Syntax parhna zaroori nahi</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Exact dono taraf · Robot cook: 20 minute vs 20 ghante</text>
  </g>

  <g transform="translate(55,719)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#2563eb"/>
    <circle cx="40" cy="36" r="18" fill="#2563eb"/><text x="40" y="43" class="n">3</text>
    <text x="68" y="44" class="t">Dividing line (VPRF)</text>
    <text x="28" y="80" class="l">Answer problem (dimaagh) vs Code problem (haath)</text>
    <text x="28" y="107" class="l">Volume · Precision · Repetition · Files: aik bhi = code</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Faisla number par ho = code problem (fee: 8 vs 11)</text>
  </g>

  <g transform="translate(55,886)">
    <rect width="715" height="155" rx="14" fill="#ffffff" stroke="#bfd3fb" stroke-dasharray="6 5"/>
    <text x="28" y="44" class="t" fill="#2563eb">Prove it in 2 minutes</text>
    <text x="28" y="80" class="l">Kharche paste karo → “Write and run code” → totals</text>
    <text x="28" y="107" class="l">Phir Groceries khud jodo: 4,250 + 2,890 + 3,120 match?</text>
    <text x="28" y="139" class="l" font-weight="600">Yahi chhota check Concept 6 ka beej hai.</text>
  </g>

  <g transform="translate(55,1053)">
    <rect width="715" height="155" rx="14" fill="#ffffff" stroke="#bfd3fb" stroke-dasharray="6 5"/>
    <text x="28" y="44" class="t" fill="#2563eb">Pichhle 2 courses se</text>
    <text x="28" y="80" class="l">Prompting: AI code tabhi chalata hai jab wording kahe</text>
    <text x="28" y="107" class="l">Markdown = # heading, - bullet · HTML = designed page</text>
    <text x="28" y="139" class="l" font-weight="600">Brief Markdown mein, report HTML mein.</text>
  </g>

  <!-- ================= PART 2 ================= -->
  <rect x="815" y="315" width="745" height="910" rx="18" fill="#ecfdf5" stroke="#059669" stroke-width="3"/>
  <text x="837" y="360" class="h" fill="#059669">PART 2 · Code commission karna</text>

  <g transform="translate(830,385)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#059669"/>
    <circle cx="40" cy="36" r="18" fill="#059669"/><text x="40" y="43" class="n">4</text>
    <text x="68" y="44" class="t">Make the AI's hands move</text>
    <text x="28" y="80" class="l">“Write and run code. Show me the code you ran.”</text>
    <text x="28" y="107" class="l">Pehle row count, column names, date range maango</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Code block nahi = code nahi chala (silent estimate)</text>
  </g>

  <g transform="translate(830,552)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#059669"/>
    <circle cx="40" cy="36" r="18" fill="#059669"/><text x="40" y="43" class="n">5</text>
    <text x="68" y="44" class="t">Brief the problem, not the program</text>
    <text x="28" y="80" class="l">Goal · Input · Output · Rules · Edge cases</text>
    <text x="28" y="107" class="l">Rules = aapka ilm · Edge: “guess mat karo, skip + list”</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Inspect → Ask → Brief · koi technical lafz nahi</text>
  </g>

  <g transform="translate(830,719)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#059669"/>
    <circle cx="40" cy="36" r="18" fill="#059669"/><text x="40" y="43" class="n">6</text>
    <text x="68" y="44" class="t">Verify work you cannot read</text>
    <text x="28" y="80" class="l">Known-answer · Reality questions · Plain-English replay</text>
    <text x="28" y="107" class="l">Adversarial pass · Cross-model check (5 checks)</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Known-answer test = firewall, kabhi skip nahi</text>
  </g>

  <g transform="translate(830,886)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#059669"/>
    <circle cx="40" cy="36" r="18" fill="#059669"/><text x="40" y="43" class="n">7</text>
    <text x="68" y="44" class="t">Errors are dialogue</text>
    <text x="28" y="80" class="l">Laal error → paste: “Diagnose it, fix, run again”</text>
    <text x="28" y="107" class="l">Wrong-but-running → symptom + expected value batao</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: 3 strikes = approach badlo, typing nahi</text>
  </g>

  <g transform="translate(830,1053)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#059669"/>
    <circle cx="40" cy="36" r="18" fill="#059669"/><text x="40" y="43" class="n">8</text>
    <text x="68" y="44" class="t">Keep the script</text>
    <text x="28" y="80" class="l">Script file + plain-English header maango</text>
    <text x="28" y="107" class="l">Brief + script + sample = aik folder (Intent Layer)</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Describe once, run forever, hand to anyone</text>
  </g>

  <!-- ================= PART 3 ================= -->
  <rect x="40" y="1255" width="745" height="580" rx="18" fill="#fff4ec" stroke="#ea580c" stroke-width="3"/>
  <text x="62" y="1300" class="h" fill="#ea580c">PART 3 · Aik masla, 5 surfaces</text>

  <g transform="translate(55,1325)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#ea580c"/>
    <circle cx="40" cy="36" r="18" fill="#ea580c"/><text x="40" y="43" class="n">9</text>
    <text x="68" y="44" class="t">Claude.ai: home surface</text>
    <text x="28" y="80" class="l">Code company ke SANDBOX mein · aapki machine safe</text>
    <text x="28" y="107" class="l">Limit: sirf uploads, temporary, har dafa upload</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Sandbox = workshop jahan jaate ho, files ka ghar nahi</text>
  </g>

  <g transform="translate(55,1492)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#ea580c"/>
    <circle cx="40" cy="36" r="18" fill="#ea580c"/><text x="40" y="43" class="n">10</text>
    <text x="68" y="44" class="t">Claude Code &amp; OpenCode</text>
    <text x="28" y="80" class="l">Terminal = folder mein baitha chat box (install ke baad)</text>
    <text x="28" y="107" class="l">Agent: files dekhta, script rakhta, schedule par chalta</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Non-programmers bhi · upload thakaye to graduate karo</text>
  </g>

  <g transform="translate(55,1659)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#ea580c"/>
    <circle cx="40" cy="36" r="18" fill="#ea580c"/><text x="40" y="43" class="n">11</text>
    <text x="68" y="44" class="t">Cowork &amp; OpenWork</text>
    <text x="28" y="80" class="l">Desktop app, terminal jitni power, andar se code</text>
    <text x="28" y="107" class="l">Plan-then-approve = plain-English replay kaam se PEHLE</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Plan parho, ghalat assumption pakro, phir approve</text>
  </g>

  <!-- ================= PART 4 ================= -->
  <rect x="815" y="1255" width="745" height="580" rx="18" fill="#f5f0ff" stroke="#7c3aed" stroke-width="3"/>
  <text x="837" y="1300" class="h" fill="#7c3aed">PART 4 · Taqat, ehtiyaat ke saath</text>

  <g transform="translate(830,1325)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#7c3aed"/>
    <circle cx="40" cy="36" r="18" fill="#7c3aed"/><text x="40" y="43" class="n">12</text>
    <text x="68" y="44" class="t">Blast radius (4 rules)</text>
    <text x="28" y="80" class="l">1 Backup copy · 2 Dry run · 3 Sab se chhota folder</text>
    <text x="28" y="107" class="l">4 Output nayi file mein · delete = recycle bin nahi</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Permission ladder: trust script ko, technology ko nahi</text>
  </g>

  <g transform="translate(830,1492)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#7c3aed"/>
    <circle cx="40" cy="36" r="18" fill="#7c3aed"/><text x="40" y="43" class="n">13</text>
    <text x="68" y="44" class="t">Edge of the map</text>
    <text x="28" y="80" class="l">Bahar: login/payment software · unattended automation</text>
    <text x="28" y="107" class="l">No-undo kaam (tax, mass email) · judgment (promotion)</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: “Code computes. You decide.” · Digital FTE</text>
  </g>

  <g transform="translate(830,1659)">
    <rect width="715" height="155" rx="14" fill="#ffffff" stroke="#d6c7fb" stroke-dasharray="6 5"/>
    <text x="28" y="44" class="t" fill="#7c3aed">4 Projects · Catch · Market of one</text>
    <text x="28" y="80" class="l">Money Detective · Grade · Books Don't Match · Photo Rescue</text>
    <text x="28" y="107" class="l">Off-the-shelf-app test: app pehle se hai = ghalat masla</text>
    <text x="28" y="139" class="l" font-weight="600">Catch = sacchi nayi baat jis par amal ho sake</text>
  </g>

  <!-- ================= BOTTOM ================= -->
  <rect x="40" y="1865" width="745" height="360" rx="18" fill="#ffffff" stroke="#e3e6ee" stroke-width="2"/>
  <text x="62" y="1907" class="bh">13 sawal → 13 jawab</text>
  <text x="62" y="1941" class="bl">1. Kaam ho sakta hai? → Bayan kar sako to</text>
  <text x="62" y="1965" class="bl">2. Code kya? → Exact dono taraf</text>
  <text x="62" y="1989" class="bl">3. Code problem? → VPRF</text>
  <text x="62" y="2013" class="bl">4. Andaza na lagaye? → “Run code”</text>
  <text x="62" y="2037" class="bl">5. Order kaise? → 5-part brief</text>
  <text x="62" y="2061" class="bl">6. Bharosa kaise? → Known-answer test</text>
  <text x="62" y="2085" class="bl">7. Error aaye? → Paste + symptom</text>
  <text x="430" y="1941" class="bl">8. Dobara kaam? → Script + brief</text>
  <text x="430" y="1965" class="bl">9. Seekhna? → Claude.ai sandbox</text>
  <text x="430" y="1989" class="bl">10. Folder mein? → Claude Code</text>
  <text x="430" y="2013" class="bl">11. App + plan? → Cowork</text>
  <text x="430" y="2037" class="bl">12. Files safe? → 4 safety rules</text>
  <text x="430" y="2061" class="bl">13. Hadd kahan? → Login, automation,</text>
  <text x="430" y="2085" class="bl">        no-undo, judgment</text>
  <rect x="60" y="2110" width="705" height="92" rx="12" fill="#eef4ff"/>
  <text x="80" y="2146" class="bl" font-weight="600">Jab phans jao: phansne ko AI ko bayan karo.</text>
  <text x="80" y="2176" class="bl">Jo skill code order karti hai, wahi project bachati hai.</text>

  <rect x="815" y="1865" width="745" height="360" rx="18" fill="#fffbeb" stroke="#f3d38a" stroke-width="2"/>
  <text x="837" y="1907" class="bh" fill="#b45309">Viva ki golden lines</text>
  <text x="837" y="1947" class="bl" font-weight="600">“You are learning to be a good client for code.”</text>
  <text x="837" y="1981" class="bl" font-weight="600">“Can I describe what done looks like?”</text>
  <text x="837" y="2015" class="bl" font-weight="600">“Code is exact, in both directions.”</text>
  <text x="837" y="2049" class="bl" font-weight="600">“Write and run code. Show me the code you ran.”</text>
  <text x="837" y="2083" class="bl" font-weight="600">“Brief the problem, not the program.”</text>
  <text x="837" y="2117" class="bl" font-weight="600">“The known-answer test is your firewall.”</text>
  <text x="837" y="2151" class="bl" font-weight="600">“Describe once, run forever, hand to anyone.”</text>
  <text x="837" y="2185" class="bl" font-weight="600">“Code computes. You decide.”</text>
</svg>
