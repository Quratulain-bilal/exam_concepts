

# viva

Is course ka ek hi sawal hai: **jab AI ko team ke kaam (workflow) mein lagana ho, to kaun sa kaam AI ko dein, kaun sa insaan ke paas rakhein, aur agar kaam kharab ho to kaise dhoondein?**

**Workflow** ka matlab hai kisi kaam ke steps jo bar bar chalte hain. Jaise: expense approval, weekly report, customer complaint.

Course ka sab se bara usool:

> **"The output is not the verdict."**
> Matlab: sirf output achha ya bura dekh kar faisla mat karo.

- Output **achha** aaya aur aap ne maan liya "ab ye step safe hai, AI ko de dein". Ye ghalti hai.
- Output **bura** aaya aur aap ne maan liya "AI ye kaam kar hi nahi sakta". Ye bhi ghalti hai.

Sahi faisla in 4 cheezon se hota hai: **kaun sa step hai, ghalti ki cost kya hai, jawab-deh kaun hai, aur problem kab shuru hui.**

# Part A: Sir ka sawal, 6 Stages alag alag

Course ke 6 stages hain: **Design, Map, Build, Diagnose, Persist, Communicate.** Har ek ko alag samjhte hain.

## Stage 1: DESIGN (kaam ko pehle design karo)

**Design kya hai?**
Tool lagane se *pehle* ye tay karna ke kaam ki asal zaroorat (requirements) kya hai, aur kaun se numbers ko calculate karna hai.

**Asaan misaal:** Ghar banane se pehle naqsha banate hain. Agar naqsha hi nahi hai to jaldi se deewarein khari kar dena bekar hai.

**Is stage ka sawal:** *"What are the actual requirements, and which numbers must be computed?"*

**Is mein 3 kaam hote hain:**
1. **Requirements nikalna.** Lamba document ya emails ko clear list mein badalna (Concept 2).
2. **Requirements par "attack" karna.** Dekhna kaun si requirement dhundli hai (Concept 2).
3. **Numbers compute karwana, likhwana nahi.** (Concept 3) Aur dekhna ke kaun si cheez AI ko di ja sakti hai (Concept 4).

## Stage 2: MAP (har step ka owner tay karo)

**Map kya hai?**
Workflow ko step by step likhna, aur har step ke saamne ye likhna: **owner kaun hai (AI, insaan, ya dono) aur wajah kya hai.** Is ko **delegation map** kehte hain.

**Asaan misaal:** Restaurant ki kitchen. Sabzi kaatna helper karta hai, magar "ye khana customer ko dena hai ya nahi" ka faisla manager karta hai. Har kaam ka owner likha hota hai.

**Is stage ka sawal:** *"For this step: can it be undone, what does an error cost, who answers?"*
Yani: kya ye undo ho sakta hai? Ghalti ki cost kya hai? Jawab-deh kaun hai?

**Ye sab se zaroori stage hai**, kyunke course ka zyada hissa (Concepts 5 se 8) isi par hai.

## Stage 3: BUILD (loop se banao)

**Build kya hai?**
Solution ek dafa mein nahi milta. Aap **4 steps ka loop** chalate hain: ideate, prototype, feedback, refine. Isi se cheez banti hai.

**Asaan misaal:** Darzi kapra seeta hai, aap ko pehna kar dekhta hai ("yahan tang hai"), phir theek karta hai. Ek hi baar mein perfect nahi hota.

**Is stage ka sawal:** *"Does this still fit in a prompt-and-iterate loop, or has it outgrown it?"*
Yani: kya ye abhi bhi chhoti baar baar prompt karne wali cheez hai, ya itni bari ho gayi ke ab engineer chahiye?

## Stage 4: DIAGNOSE (kharabi ki wajah dhoondo)

**Diagnose kya hai?**
Jab AI ka output kharab aaye, to **randomly cheezein badalne ke bajaye** pehle ye dekhna ke symptom kab shuru hua. Phir us se wajah ka andaaza lagana.

**Asaan misaal:** Doctor pehle poochta hai "ye dard kab se hai?", phir dawa deta hai. Bina poochhe dawa nahi.

**Is stage ka sawal:** *"When did the symptom first appear?"*

Is mein 4 wajohat (causes) hain aur 5 steps ka sequence. Wo Part B mein alag alag samjhaye hain.

## Stage 5: PERSIST (fix ko hamesha ke liye rakho)

**Persist kya hai?**
Jo fix aap ne dhoondha, usay **chat mein chhorne ke bajaye configuration mein daal dena**, taake agli dafa (aap ke liye ya kisi aur ke liye) wo khud kaam kare. Is ko **promotion** kehte hain.

**Asaan misaal:** Aap ne ek recipe ka raaz seekha. Agar sirf zehan mein rakha to aap ki chhutti par koi nahi jaanta. Agar recipe book mein likh diya to sab ke kaam aayega.

**Is stage ka sawal:** *"Is this fix a rule, a reference, or a procedure?"*
Ye 3 chizein Part B mein alag samjhaunga.

## Stage 6: COMMUNICATE (sach bol kar batao)

**Communicate kya hai?**
Doosron ko (manager, client, risk team) batana ke AI workflow kya karta hai. **Value bhi batao aur limits bhi**, aur batao ke **insaani check (human gate) kahan hai.**

**Asaan misaal:** Gaari bechte waqt sirf "bohat tez hai" nahi kehte. Ye bhi batate hain "brake yahan hai". Isse customer ka bharosa barhta hai.

**Is stage ka sawal:** *"What does it do, and where exactly is the human gate?"*

**Yaad rakhne wali baat:** Source kehta hai stakeholders AI workflow par **zyada** bharosa karte hain jab human checkpoints saaf bataye jayen, kam nahi.

## Six stages ek line mein

| # | Stage | Ek line mein |
|---|---|---|
| 1 | Design | Pehle zaroorat likho, numbers compute karwao |
| 2 | Map | Har step ka owner aur wajah likho |
| 3 | Build | Loop se banao, bara ho jaye to engineer ko do |
| 4 | Diagnose | Symptom kab aaya, us se wajah dhoondo |
| 5 | Persist | Fix ko configuration mein daalo |
| 6 | Communicate | Kya karta hai batao, human gate batao |

**Poori ek line yaad karein:** *"Requirements settle karo, har step ko three criteria se map karo, loop se banao, timing se diagnose karo, fix ko configuration mein rakho, phir batao ye kya karta hai aur gate kahan hai."*

# Part B: Jahan 3, 4 ya 5 points hain, wahan har point alag

Ab wo saari lists jo viva mein "kitni hain aur kaun si hain" ke tor par poochi ja sakti hain.

## B1. Teen decisions (har step par)

Har step par **3 alag faisle** hote hain. Inhein mix karne se galat map bantay hain.

1. **Eligibility (kya AI is ko chhoo sakta hai?).** Isme 2 gates hain:
   - **Data gate:** kya ye data is tool mein daalna jaiz hai? (ye Governance course ka sawal hai)
   - **Input gate:** kya step ki saari zaroorat model ko di ja sakti hai? (window test)
   - Agar kisi gate par "nahi" aaya, to baat wahin khatam.
2. **Ownership (owner kaun hoga?).** Iska faisla **teen criteria** (B2) karte hain.
3. **Implementation (kaun si cheez ise uthaye?).** Ye sab se aakhir mein tay hota hai, aur sirf unn steps ke liye jo pehle do faisle paas kar chuke hon.

**Zaroori baat:** "Ye number compute karna hai" sirf implementation wali baat hai (code execution). Ye is baat ka sabab nahi ke step AI ko dein. Isi ghalti se high-stakes calculation bina review ke reh jati hai.

## B2. Teen criteria (owner tay karne ke liye)

Ye teen sawaal step ke baare mein hain, model ke baare mein nahi. **Sirf yehi teen.**

**1. Reversibility (undo ho sakta hai?)**
- Matlab: agar AI ghalti kare to kya wapas theek kar sakte hain?
- Misaal: draft dobara likha ja sakta hai (theek). Bheji hui email unsend nahi hoti (mushkil).
- Asool: jo undo ho sakta hai, usay delegate karna aasan hai.

**2. Stakes (ghalti ki cost)**
- Matlab: **bure case mein** ghalti ki qeemat kya hai? Average ya "aam tor par" nahi.
- Misaal: galat label lagne se ek minute zaya hota hai. Galat penalty figure ki cost poori penalty hai.

**3. Accountability (jawab-deh kaun hai)**
- Har step ka koi na koi jawab-deh hota hai, isliye sirf ye kehna kafi nahi.
- Asal sawal ye hai: **kya ye step khud wo faisla hai jiska banda jawab deta hai, ya ye ek input hai jise koi judge karta hai?**
  - Agar step ek **input** hai jise koi aage judge karta hai, to delegate ho sakta hai.
  - Agar step khud **faisla** hai, to delegate nahi ho sakta.
- Accountability kabhi machine par nahi jati, kyunke machine se poocha nahi ja sakta.

**Teen baatein jo examiner pooch sakta hai:**
- **Score nahi, teen sawal hain.** Teeno ko jama nahi karte. Aam tor par ek criterion step ka faisla karta hai aur baaki do uski taeed karte hain. Aap ko wo ek criterion naam se batana chahiye.
- **Jab teeno mein ikhtilaf ho** to sab se **strict** wala jeetta hai.
- **Criterion nahi hai:** "AI ne pehle is par kitna acha kaam kiya". Ye nahi chalta (isi se halo delegation hoti hai, B4).

## B3. Teen classifications (step ka owner kaun?)

Har step in 3 mein se ek hota hai:

1. **AI-appropriate:** AI own kar sakta hai. Kyunke ye undo ho sakta hai aur koi aage judge karta hai.
2. **Human-retained:** insaan poori tarah own karta hai. (jaise "sign and send")
3. **Collaborative:** AI banata hai, **naam wala insaan judge karta hai.** Jis lamhe koi judge nahi karta, ye collaborative nahi rehta.

**Misaal (contract review):**
- Clauses nikalna: AI
- Redline draft karna: Collaborative
- Har change approve karna: Human
- Sign and send: Human

## B4. Teen mapping errors (map kaise ghalat hota hai)

Teeno ghalatiyan us waqt **reasonable lagti hain.** Isi liye khatarnaak hain.

**1. Halo delegation**
- Matlab: pichla step acha gaya, is liye agla step bhi AI ko de diya.
- Misaal: "AI ki summaries sahi thi, to severity classification bhi AI karega." Summary aur classification do alag steps hain.
- Yaad rakhein: *"Drafting quality is evidence about the draft. It is not evidence about the decision."*

**2. Unstaffed gate**
- Matlab: review naam ki reh gayi. Pehle review hota tha, phir sirf glance, phir bas click.
- Misaal: manager har Friday queue ko ek hi baar mein approve kar deta hai, kisi case ko khole bina. Map abhi bhi "collaborative" kehta hai magar asal mein step automated ho chuka hai.
- Map isay nahi batata, kyunke map wo likhta hai jo *design* kiya tha, wo nahi jo *chal raha hai*.

**3. Mapping the tool instead of the work**
- Matlab: team apni pasandeeda feature ke mutabiq workflow banati hai, kaam ke mutabiq nahi.
- Misaal: ek acha Skill hai, to workflow mein us Skill jaisa step shaamil kar liya.
- Ye teeno mein sab se mushkil se nazar aata hai.

**Over-delegation** in teeno ki chhatri hai: AI ko step ke risk se zyada de dena.

**Check karne ka order:** pehle bina tools ke kaam map karo, har step alag classify karo, phir har collaborative step par poocho "reviewer kaun hai aur kab karta hai?"

## B5. Teen cheezein jo chupke se kharab hoti hain

Source ke mutabiq 3 controls waqt ke saath decay karte hain, aur **kharab hone ke waqt koi signal nahi aata.**

1. **Review gate** (reviews glance aur phir click ban jati hain)
2. **Standing instruction** (output dheere dheere rule se hat jata hai)
3. **Map khud** (wo workflow batata hai jo ab koi nahi chalata)

**Hal:** ek **scheduled read** (tay shuda tareekh par review).

**Map ko 2 cheezein chahiye:**
- **Map owner:** ek naam wala banda (team nahi).
- **Review date:** aam tor par quarterly.

## B6. Map review ke 4 sawaal (20 minute)

1. Kya koi step add ya remove hua jo map par nahi?
2. Har collaborative step ko **pichle hafte** kis ne review kiya aur kitni der? (agar koi nahi bata sakta, to step automated hai)
3. Kya volume ya stakes badle? (20 cases ke liye bana gate 50 par fail ho sakta hai)
4. Kya har configuration abhi current hai? (Skills, knowledge sources, standing instructions)

Sawal 2 asal masle pakarta hai, kyunke ye *pichle hafte* ke baare mein hai, policy ke baare mein nahi.

## B7. Implementation ke 5 "carriers" (kaun si cheez kaam uthaye)

| Step kya hai | Kaun uthaye | Kyun |
|---|---|---|
| Repeatable procedure, fixed steps | **Skill** | Sab ke liye same chalta hai |
| Rules/reference jo hamesha chahiye | **Project knowledge** | Har run mein paste nahi karna |
| Calculation jis par output depend karta hai | **Code execution** | Compute hota hai, likha nahi jata |
| Har output par lagne wali constraint | **Standing instruction** | Kisi ko yaad nahi rakhna parta |
| Wo step jo insaan own kare | **Named review gate** | Ek banda, ek lamha, ek cheez check karne ko |

Insaan wale step ko sirf "human" likhna kafi nahi. Chahiye: **naam, waqt, aur kya check karna hai.**

## B8. Bure output ki 4 wajohat (timing se pehchano)

Sab se pehle ye poochein: **symptom kab aaya?**

**1. Under-specification (prompt mein kami)**
- Symptom: pehle hi jawab se ghalat.
- Matlab: prompt mein wo cheez thi hi nahi jo step ko chahiye thi.
- Test: prompt dobara parhein. Kya missing cheez waqai us mein hai?
- Fix: jo choota use add karein.
- Ye sab se aam wajah hai aur sab se sasta fix.

**2. Context overload (baat lambi ho gayi)**
- Symptom: shuru theek tha, phir kharab hota gaya.
- Matlab: conversation context window se lambi ho gayi, isliye purani cheezein chhoti ya gir gayi aur early instructions kamzor ho gayin.
- Test: nayi session mein wohi instruction dohrain. Kya ab theek chalta hai?
- Fix: restart karein ya summary banayein. Behtar prompt yahan kaam nahi karta.

**3. Wrong feature or model (ghalat tool)**
- Symptom: ek hi qism ki ghalti baar baar.
- Misaal: numbers thode ghalat aate hain (calculation prose mein maangi gayi). Ya gehra kaam ho aur tier tez magar sasta chuna gaya ho.
- Test: wohi step sahi feature ya mazboot tier par ek baar chalayein.
- Fix: feature ya tier badlein.

**4. Stale configuration (purani setting)**
- Symptom: "pehle theek chalta tha, ab nahi."
- Matlab: koi saved instruction, file ya Skill purani ho gayi.
- Misaal: pichle quarter ke figures knowledge base mein hain aur is quarter ki report unhein quote karti hai.
- **Ye silent hai.** Koi error nahi aata.
- Fix: configuration ki maintenance.

**5th cheez (cause nahi, last resort): Expectation mismatch**
- Task hi aisa hai jo tool kar nahi sakta. Misaal: "agle quarter ki exact sales figure batao."
- Ye sirf tab sahi hai jab pehli 4 wajohat rule-out ho chuki hon.
- Fix task ko badalna hai: range maango with assumptions, ya adjustable model.

**Zaroori note:** timing sirf ye batati hai ke **pehle kahan dekhna hai**, ye nahi ke wajah kya hai. Ek timing ki ek se zyada wajah ho sakti hai.

## B9. Diagnostic sequence (5 steps, sasta pehle)

Is order mein check karein, "task fit nahi" kehne se pehle:

1. **Prompt dobara parho.** 5 hisson ke against: role, context, task, constraints, format.
2. **Conversation ki lambai dekho.** Overload to nahi? Restart ya summary.
3. **Feature aur model dekho.** Calculation ho to code execution? Mushkil kaam ho to speed tier to nahi?
4. **Configuration current hai?** Instructions, knowledge, Skills.
5. **Sirf ab:** kya task fit hai bhi?

Isko ek seedhi (ladder) samjhein: sasta check upar, mehnga neeche. **Zyada log ulta chalte hain**: seedha sab se mazboot model ya "task impossible" par jump karte hain.

**Prompt ke 5 parts** (step 1 ke liye): Role, Context, Task, Constraints, Format. Ye isliye slot ba slot check hote hain kyunke likhne wale ko prompt theek lagta hai (missing cheez uske zehan mein hoti hai).

## B10. Build loop ke 4 steps

1. **Ideate:** options banana.
2. **Prototype:** ek option ko itna concrete banana ke us par reaction de sakein.
3. **Feedback:** dekhna kya ghalat hai (jo pehle se pata nahi hota).
4. **Refine:** usay theek karna. Phir doosra round.

Loop ko ek **Project** mein chalayein taake background aur purane faisle stable rahein. Alag alag chats mein har round thodi alag samajh se shuru hota hai.

**Source ka 3 cycle ka example (dashboard artifact):**
- Cycle 1: 5 charts ban gaye. (aasan)
- Cycle 2: filter aur totals maange. Filter chala, **totals ghalat.** Wajah: totals likhe gaye the, compute nahi hue. Ye feature problem tha, behtar description se hal nahi hota.
- Cycle 3: color aur print layout. Pehli dafa mein chal gaya. Ye description problem tha.

**Hunar:** description problem aur feature problem mein farq karna.

## B11. Escalation ke 2 signals (jo ek jaise lagte hain)

| Signal | Matlab | Kahan jaana hai |
|---|---|---|
| **Doosre log ab is par depend karte hain** | Ye infrastructure ban gaya | Developer/architect |
| **Maine ye teen baar ek hi tareeqe se hal kiya** | Shape stable hai, manufacture ho sakta hai | "From One-Off to Worker" course |

Pehla signal ye batata hai **kaun exposed hai.** Dusra ye batata hai **tareeqa ab badal nahi raha.**
Escalate karna **sahi jawab hai**, nakami nahi. Nakami ye hai ke aap prompt se chalate rahein jab ke doosre depend karne lagein.

## B12. Fix ke 3 ghar (rule, reference, procedure)

Poochein: *"Kya ye correction dobara chahiye hogi?"* Agar haan, to **promotion** (configuration mein le jaana).

1. **Rule** → **Standing instruction.** Wo limit jo hamesha lagti hai.
   Misaal: "Pehli line mein target segment zaroor likho."
2. **Reference** → **Knowledge base.** Wo material jo kaam ko parhna padta hai.
   Misaal: brand voice guide, current product list.
3. **Procedure** → **Skill.** Steps ka order.
   Misaal: "Weekly report is exact format mein, is order mein banao."

**Galat ghar mein daalne ke nuqsan:**
- Procedure ko ek line ki instruction bana do, to order kho jata hai.
- Reference ko standing instruction mein thoon do, to har prompt bhari ho jata hai.

**Source ka example:** analyst har mahine chat mein likhta tha "cancelled orders exclude karo". Wo chhutti par gaya, colleague ne report chalayi, aur cancelled orders shaamil ho gaye. Fix tha, magar aisi jagah jahan sirf ek banda dhoondh sakta tha.

**Memory kaafi kyun nahi?** Memory per-user hai (colleague ko nahi milti) aur best-effort hai (aap use point ya hand over nahi kar sakte). Configuration shared aur parhne ke qabil hai.

## B13. Friction ke 3 signals aur 2 moves

**Friction** = chhota, bar bar hone wala kharcha jo aap ne dekhna chhor diya.

**Teen signals:**
1. **Repetition:** har run mein wohi cheez paste/type karna. Fix: saved context ya standing instruction.
2. **Correction:** har output mein wohi ghalti theek karna. Fix: configuration change taake wo aaye hi nahi.
3. **Variance:** alag log wohi kaam karen to alag result. Fix: shared Skill ya knowledge base. (Ye signal sab se kam nazar aata hai kyunke koi ek banda isay mehsoos nahi karta, ye sirf reviewer ke paas dikhta hai.)

**Do moves (is order mein):**
1. **Consolidate:** teen prompts ko ek mein milana jo har dafa wohi background maangte hain.
2. **Promote:** repeated pattern ko configuration mein daalna.

Pehle consolidate kyun? Kyunke jo step merge hone wala hai, usay promote karna zaya mehnat hai.

## B14. Measure ke teen hisse

**1. Baseline (pehle ki naap).** Badalne se *pehle* workflow ek baar waisa hi chalayein aur 3 numbers likhein: **time, revision rounds, manual steps.** Baad mein baseline nahi ban sakti, kyunke purane tareeqe ka aap ka andaza aap ko flatter karega.

**2. Chaar metrics (matching karke):**

| Workflow kaisi hai | Kis par optimise karein | Kyun |
|---|---|---|
| Internal draft | **Time** | Speed ahem hai, chhoti ghalti sasti |
| Customer ko jane wali report | **Consistency** | Alag formats bharosa torte hain |
| Compliance ya finance output | **Accuracy** | Ek ghalat figure ek ghante se mehnga |
| Kai logon ka kaam | **Variance** | Kharcha logon ke beech mein hota hai |

Metric pehle se tay karne se ye bhi pata chalta hai ke kab rukna hai.

**3. Parallel run.** Do-teen cycles purana aur naya saath chalana. Teen faide: evidence, fallback, aur un logon ki razamandi jinka kaam badla.

**Cost batana:** cost = AI tool ki cost + insaani waqt (jo gates rakhe). Saving = baseline × kitni dafa chalta hai × kitne log chalate hain. Misaal: 20 minute/hafta × 3 analysts ≈ 50 ghante/saal. Aur wo risk bhi batayein jo gates ke baad bhi bacha hai.

## B15. Bura output nikal jaye to: 4 faisle (pehle se tay)

Is ko **incident path** kehte hain. Faisle design ke waqt hote hain, ghalti ke waqt nahi.

1. **How it gets stopped:** workflow ko sab se tezi se kaun rok sakta hai, aur kya use permission chahiye?
2. **What is already out:** kitne outputs affect hue aur kahan gaye? (stale configuration ek nahi, us din ke baad ka har result kharab karti hai.)
3. **Who is told, and by when:** customer, internal owner, risk/compliance. Late disclosure bohat mehnga hota hai.
4. **What changes in the map:** kaun si cause thi? Step ghalat classify hua ya gate staff nahi tha? Map mein tareekh ke saath tabdeeli likhein.

Faisle **1 aur 4** workflow designer ke hain aur design time par ya kabhi nahi.

## B16. Communicate: 3 jumle jo galat hain, aur 3 version

**Teen overstating phrases (jo bharosa torte hain):**
1. **"Fully automated."** Lagbhag kabhi sach nahi.
2. **"AI handles X."** Human gate jumle se ghayab ho jata hai.
3. **"It's basically as good as a person at Y."** Aisa maiyar jo tool kabhi na kabhi miss karega.

**Hal:** *state what the tool does, then name the human checkpoint.* Jab audience bharosa karne ka faisla kar rahi ho to teesri baat bhi: **say what it refuses** (wo cases jo tool hand over karta hai).

**Ek workflow, teen audiences:**
- **Legal lead:** mechanism aur failure modes chahiye.
- **Practice executive:** outcome aur oversight (e.g. turnaround 2 din se aadha din).
- **Client ka risk function:** control. ("Har term ek qualified lawyer approve karta hai.")

Teeno mein gate shaamil hai.

## B17. Requirements ke 5 jawab (task definition)

Business need ko 5 saaf jawabon mein badlein:
1. **What** is produced?
2. **For whom?**
3. **How often?**
4. **From what data?**
5. **In what format?**

Jo jawab missing hai, wo clarifying question hai jo aap ke zimme hai, model ke bharne ka blank nahi.

## B18. Research ke 2 qisam ke sawal

1. **Stable concept ya method:** model ki apni knowledge theek hai.
2. **Current, priced ya dated:** aisa source maango jo aap khol saken (answer **aur link**).

# Part C: Kya agle step mein karna chahiye?

Ab maine saari concepts aur lists alag alag, simple tareeqe se de di hain. Agar aap theek samjhein to agla step ye ho sakta hai:

1. **Viva Q&A** ab isi aasan style mein (har sawal ka jawab pehle chhota, phir wajah, phir misaal).
2. **Scenario questions** (jaise "ek team ne ye kiya, kaun si ghalti hai?") ke model answers.
3. **Rapid-fire** aur **last-minute revision sheet.**

Aap bata dein pehle kaun sa chahiye. Agar kisi ek point ko aur aasan karna hai, jaise "halo delegation" ya "unstaffed gate" ko misaal ke saath dobara, to uska naam likh dein.
Ab flow "**problem → uska solution → phir naya problem → uska solution**" ke style mein hai. Har step mein dikhega ke **kya masla hua** aur **kis concept ne usay solve kiya**. Definitions bhi wahin saath hain.

## Block 1: Shuruat se Design tak

```
===============================================================
 PROBLEM --> SOLUTION FLOW (upar se neeche chalein)
===============================================================

[P1] PROBLEM: "Main AI use karta hoon" = personal habit.
     Mood se badalti hai, aap chhutti par gaye to khatam.
     |
     v
[S1] SOLUTION: WORKFLOW + STEP
     WORKFLOW = team ka repeatable process
     STEP = workflow ka ek named hissa, jiska EK owner ho
     (session baad mein judge hota hai, step PEHLE decide)
     |
     v
[P2] PROBLEM: Do teams, same tool, same model (contract review).
     Team 1 sahi steps AI ko diye = kaam chala.
     Team 2 approval bhi AI ko di = 1 mahine mein tool band.
     Ab output dekh kar galat conclusion nikalte hain:
       acha output  -> "step safe hai" (GALAT)
       bura output  -> "task impossible hai" (GALAT)
     |
     v
[S2] SOLUTION: "THE OUTPUT IS NOT THE VERDICT"
     Faisla 4 cheezon se: kaun sa step / ghalti ki cost /
     jawab-deh kaun / symptom KAB shuru hua
     (REDLINE = marked-up version jo wanted changes dikhata)
     |
     v
[P3] PROBLEM: Kaam shuru kahan se karein? Request vague hai
     ("better reporting chahiye") ya 40 page ka messy document.
     |
     v
[S3] SOLUTION: REQUIREMENTS EXTRACTION + TASK DEFINITION
     RFP = khareedar ka bid maangne wala document
     AI se TABLE maango: label | section | answered? | ambiguous?
     (summary nahi, structure, taake koi bhi check kar sake)
     TASK DEFINITION = need ko 5 jawabon mein badlo:
       WHAT / FOR WHOM / HOW OFTEN / FROM WHAT DATA / WHAT FORMAT
     Jo jawab missing = clarifying question (model na bhare)
     |
     v
[P4] PROBLEM: Extraction sirf wo dhoondti hai jo LIKHA hai,
     wo nahi jo MATLAB tha. Do teams alag cheez bana dein
     ("report promptly deliver ho" = 2 din ya 2 hafte?)
     |
     v
[S4] SOLUTION: ATTACK THE REQUIREMENTS
     3 sawal: kaun ambiguous? kaun si 2 log alag parhen?
     kaun si indirectly implied?
     TEST: kya iska CHECK likh sakte ho? Nahi = abhi vague
     Faida: 1 clarifying question vs poora kaam zaya
     |
     v
[P5] PROBLEM: Plan ke numbers. Likha hua number aur calculate
     kiya hua number PAGE par ek jaise dikhte hain.
     Totals ghalat nikle magar sahi lagte the.
     |
     v
[S5] SOLUTION: COMPUTE, NEVER WRITE
     SYNTHESIS = considerations jama kar ke options banana
       (AI isme acha hai)
     CODE EXECUTION = assistant code likh kar chalata hai aur
       batata hai kya compute hua (4th output format)
     Pehle COMPUTE, phir RECOMMEND, assumptions ke saath
     Limit: code ghalat column utha sakta hai, to check karo
     KYA compute hua
     |
     v
[P6] PROBLEM: Recurring kaam (RFP) har dafa naye sire se
     setup karna parta hai.
     |
     v
[S6] SOLUTION: PROJECT + 3 saved cheezein
     PROJECT = ek kism ke kaam ka saved workspace
     KNOWLEDGE BASE = files jo Project parh sakta hai
     STANDING INSTRUCTION = rule jo har run par lagta hai
     SKILL = saved procedure, har dafa same tareeqe se
     (Skill account level par, baaki Project par)
     |
     v
```

## Block 2: Map ka flow (Context test, 3 criteria)

```
[P7] PROBLEM: Plan useless nikla. Operations lead ne headcount
     manga, AI ne 3 hire karne ko kaha. Magar hiring freeze
     meeting mein decide hua tha, dataset mein nahi tha.
     Model ne gap "aam tor par aisa hota hai" se bhara.
     |
     v
[S7] SOLUTION: WINDOW TEST (context test)
     "Step ki SAARI zaroorat window mein rakh sakta hoon?
      Nahi, to step MERA hai."
     CONTEXT = jo model ko dikhta hai (prompt + files +
       conversation)
     CONTEXT WINDOW = ek waqt mein kitna context sambhal
       sakta hai, uski hadd
     JUDGMENT STEP = jis ka input aap supply nahi kar sakte
       (hiring freeze, risk appetite, client ka delay)
     RESEARCH: stable concept = model theek.
       Current/priced/dated = source maango jo KHOL sako
     |
     v
[P8] PROBLEM: Har step par teen alag faisle mix ho jate hain,
     to map reasonable lagta hai magar ghalat hota hai.
     |
     v
[S8] SOLUTION: 3 DECISIONS alag alag
     1 ELIGIBILITY: kya AI chhoo sakta hai? (2 gates)
        Gate A: DATA GATE (kya ye data tool mein jaiz hai?
                Governance course)
        Gate B: Window test (upar wala)
        Kisi gate par "nahi" = step HUMAN ka
     2 OWNERSHIP: owner kaun? (agla step, 3 criteria)
     3 IMPLEMENTATION: kaun si cheez uthaye? (sab se AAKHIR)
     |
     v
[P9] PROBLEM: Owner kaun ho? "AI ne achha kiya" ya "lagta hai
     important" jaisi wajohat se faisle hote hain.
     |
     v
[S9] SOLUTION: 3 CRITERIA (sirf ye 3)
     1 REVERSIBILITY: ghalti ho to UNDO ho sakta hai?
     2 STAKES: BURE case mein ghalti ki cost (average nahi)
     3 ACCOUNTABILITY: kya YE step khud wo faisla hai jiska
       banda jawab deta hai? Ya wo INPUT jo koi aage judge
       karta hai? (machine par kabhi nahi jati)
     RULES: ek criterion decide karta hai, uska NAAM likho |
       ikhtilaf ho to STRICTEST jeetta hai | "AI pehle acha
       tha" criterion NAHI hai
     |
     v
[P10] PROBLEM: Criteria laga diye, ab step ko label kya dein?
     |
     v
[S10] SOLUTION: 3 CLASSES
     AI-APPROPRIATE : AI own kare (undo ho sake + koi judge kare)
     COLLABORATIVE  : AI banata hai, NAAM wala insaan judge
                      karta hai (judge band = collaborative khatam)
     HUMAN-RETAINED : insaan poori tarah own kare
     DELEGATION MAP = poora workflow, har step ka owner + wajah
     |
     v
[P11] PROBLEM: Step AI ko diya, magar AI ISE kaise karega?
     "Compute karna hai" ko ownership ka sabab bana liya.
     |
     v
[S11] SOLUTION: IMPLEMENTATION table (5 carriers)
     fixed procedure ............ SKILL
     rules/reference ............ PROJECT KNOWLEDGE
     calculation ................ CODE EXECUTION
     har output par constraint .. STANDING INSTRUCTION
     insaani step ............... NAMED REVIEW GATE
                                 (naam + waqt + kya check)
     "Compute karna hai" = implementation, AI ko dene ki wajah nahi
     |
     v
```

## Block 3: Map ki ghaltiyan, Build, Diagnose

```
[P12] PROBLEM: Map banne ke baad bhi 3 ghaltiyan aati hain,
     aur teeno us waqt REASONABLE lagti hain.
     |
     v
[S12] SOLUTION: 3 ERRORS ko pehchano
     OVER-DELEGATION = step ke risk se ZYADA AI ko dena
       (ye teeno ki chhatri hai)
     1 HALO DELEGATION: pichla step acha gaya, isliye agla bhi
       de diya. "Drafting quality draft ka evidence hai,
       decision ka nahi."
     2 UNSTAFFED GATE: review glance phir click ban gaya.
       Map nahi batata (map DESIGN likhta hai, jo CHAL raha hai
       wo nahi)
     3 MAPPING THE TOOL INSTEAD OF THE WORK: feature ke mutabiq
       workflow, kaam ke mutabiq nahi
     CHECK ORDER: bina tools ke map -> har step alag classify
       -> har collaborative step par "reviewer kaun, kab?"
     |
     v
[P13] PROBLEM: Map waqt ke saath chupke se ghalat ho jata hai.
     Gate, standing instruction, map khud: teeno decay hote
     hain aur koi alarm nahi bajta.
     |
     v
[S13] SOLUTION: MAP OWNER + SCHEDULED READ
     MAP OWNER = ek NAAM wala banda (team nahi)
     SCHEDULED READ = tay tareekh par review (quarterly)
     4 SAWAAL (20 min):
       1 koi step add/remove hua jo map par nahi?
       2 har collaborative step ko PICHLE HAFTE kis ne review
         kiya aur kitni der? (koi nahi bata sake = automated)
       3 volume/stakes badle? (20 case ka gate 50 par fail)
       4 har configuration current hai?
     |
     v
[P14] PROBLEM: Ek prompt se solution nahi milta. Aap use
     "vending machine" samajhte hain.
     |
     v
[S14] SOLUTION: BUILD LOOP (Project ke andar)
     IDEATE (options banao) -> PROTOTYPE (itna concrete ke
     reaction de sako) -> FEEDBACK (kya ghalat, jo pehle pata
     nahi) -> REFINE (theek karo) -> dobara
     ARTIFACT = chat ke andar bana chhota working web page
     Hunar: description problem vs feature problem pehchano
     (totals ghalat = feature problem, color/print = description)
     |
     v
[P15] PROBLEM: Chhota tool 6 mahine baad 3 departments
     use kar rahe hain, aur board report mein jaa raha hai.
     |
     v
[S15] SOLUTION: ESCALATION SIGNAL
     ESCALATION SIGNAL = doosre log depend karne lagen
     (uptime, access, "kisko bulayein" chahiye)
     2 signals:
       "others depend on this" -> developer/architect
       "same tareeqa 3 baar"   -> From One-Off to Worker
     Escalate karna sahi jawab hai, nakami nahi
     |
     v
[P16] PROBLEM: Output kharab aaya. Log ya to haar maan lete
     hain ("tool nahi kar sakta") ya randomly cheezein badalte
     hain.
     |
     v
[S16] SOLUTION: Poocho "SYMPTOM KAB SHURU HUA?"
     (timing batati hai PEHLE kahan dekho, cause nahi)
     4 CAUSES:
     1 UNDER-SPECIFICATION: pehle jawab se ghalat. Prompt mein
       wo cheez thi hi nahi. Fix: kami add karo
     2 CONTEXT OVERLOAD: shuru theek, phir kharab. Fix: restart
       ya summary (behtar prompt kaam nahi karta)
     3 WRONG FEATURE OR MODEL: ek hi qism ki ghalti baar baar.
       TIER = model version (fast/cheap se slow/capable)
       Fix: sahi feature ya sahi tier
     4 STALE CONFIGURATION: "pehle chalta tha". Koi error nahi
       (SILENT). Fix: configuration maintenance
     |
     v
[P17] PROBLEM: Kya pehle check karein? Log seedha bara model
     ya "task impossible" par jump karte hain.
     |
     v
[S17] SOLUTION: DIAGNOSTIC SEQUENCE (sasta pehle, 5 steps)
     1 prompt dobara parho: ROLE, CONTEXT, TASK, CONSTRAINTS,
       FORMAT
     2 session ki lambai
     3 feature + model
     4 configuration current?
     5 SIRF AB: kya task fit hai?
     EXPECTATION MISMATCH = task aisa jo tool nahi kar sakta
       (exact future number). Pehle 4 rule-out hon.
       Fix task badlo: range + assumptions
     |
     v
```

## Block 4: Persist, Operate, Communicate

```
[P18] PROBLEM: "Too generic" ya "not quite right" jaisi
     reaction se agla attempt sirf guess hota hai.
     |
     v
[S18] SOLUTION: REACTION -> INSTRUCTION
     Poocho: "Kya present hota to sahi hota, aur setup ka
     konsa hissa (LEVER) isay control karta hai?"
     Lever: prompt / standing instruction / knowledge
     Lever na mile = abhi sirf reaction hai
     |
     v
[P19] PROBLEM: Fix mil gaya magar chat mein reh gaya.
     Analyst har mahine "cancelled orders exclude karo" likhta
     tha. Chhutti par gaya, colleague ne report chalayi,
     numbers galat gaye.
     |
     v
[S19] SOLUTION: PROMOTION + RULE / REFERENCE / PROCEDURE
     PROMOTION = fix ko chat se configuration mein le jana
     Test: "kya ye dobara chahiye hogi?" Haan = promote
     RULE (hamesha lagne wali limit) -> STANDING INSTRUCTION
     REFERENCE (material jo parhna hai) -> KNOWLEDGE BASE
     PROCEDURE (steps ka order) -> SKILL
     Galat ghar: procedure 1 line mein = order kho jata hai;
     reference instruction mein = har prompt bhari
     Memory kaafi nahi: per-user aur best-effort hai
     |
     v
[P20] PROBLEM: Chhote bar bar hone wale kharche jo dikhte
     hi nahi (2 minute ka reformat, saal mein 50 dafa).
     |
     v
[S20] SOLUTION: FRICTION dhoondo, phir 2 moves
     FRICTION = chhota repeated cost jo dekhna chhor diya
     3 SIGNALS:
       1 REPETITION: wohi paste/type har run
       2 CORRECTION: wohi flaw har output mein theek karna
       3 VARIANCE: alag log, alag result (sirf reviewer ko
         dikhta hai)
     2 MOVES (is order mein): CONSOLIDATE (steps milao)
       phir PROMOTE (pattern configuration mein)
     |
     v
[P21] PROBLEM: Improvement ko sabit kaise karein? "45 se 25
     minute" tabhi kehne ke qabil jab pehle naapa ho.
     |
     v
[S21] SOLUTION: MEASURE
     BASELINE = badalne se PEHLE ki naap: time, revision
       rounds, manual steps (baad mein nahi ban sakti)
     1 METRIC chuno: time (internal draft) | consistency
       (customer report) | accuracy (compliance/finance) |
       variance (kai log)
     PARALLEL RUN = purana + naya saath, 2-3 cycles
     COST = AI tool + bacha hua insaani waqt (gates)
     SAVING = baseline x kitni dafa x kitne log
     + wo risk jo gates ke baad bhi bacha
     |
     v
[P22] PROBLEM: Sab kuch kar ke bhi kabhi na kabhi bura output
     bahar nikal jata hai. Aur us ghante mein sab improvise
     hota hai.
     |
     v
[S22] SOLUTION: INCIDENT PATH (4 faisle PEHLE se)
     1 STOP: kaun rok sakta hai, bina permission ke?
     2 SCOPE: kitne outputs affect hue, kahan gaye?
     3 TELL: kis ko, kab tak? (late disclosure mehnga)
     4 MAP CHANGE: kaun si cause thi? Tareekh ke saath tabdeeli
     (1 aur 4 designer ke, design time par ya kabhi nahi)
     |
     v
[P23] PROBLEM: Doosron ko batate waqt log overstate kar dete
     hain, aur pehli visible ghalti par bharosa toot jata hai.
     |
     v
[S23] SOLUTION: COMMUNICATE: kya karta hai + GATE ka naam
     3 GALAT JUMLE:
       1 "Fully automated" (lagbhag kabhi sach nahi)
       2 "AI handles X" (human gate ghayab)
       3 "As good as a person" (aisa maiyar jo miss hoga)
     SAHI: kya karta hai + HUMAN CHECKPOINT + "say what it
       REFUSES" (wo cases jo person ko dete hain)
     3 AUDIENCES, har ek mein gate:
       legal lead  -> mechanism aur failure modes
       executive   -> outcome aur oversight
       risk team   -> control
     Gate saaf batao = bharosa BARHTA hai
     |
     v
===============================================================
 EK LINE: Output verdict nahi hai. Step ko cost aur jawab-deh
 se judge karo, aur failure ko is se ke WOH KAB shuru hui.
===============================================================
```
through story



Theek hai, ab main isko ek **kahani ki tarah, paragraph by paragraph** likhta hoon. Har naya term jahan pehli dafa aata hai, wahin uski definition bhi saath hai. Bas upar se neeche parhte jayein.

## Kahani 1: Ye sab shuru kyun hua?

Pehle samjhein ke **workflow** kya hai. Workflow kisi kaam ke woh steps hain jo team bar bar chalati hai, jaise expense approval, weekly report ya customer complaint. Aur **step** workflow ka ek named hissa hota hai jiska **sirf ek owner** hota hai.

Ab masla ye hai ke bohat log kehte hain "main AI use karta hoon". Ye sirf ek **personal habit** hai. Ye aap ke mood par chalti hai, aur aap chhutti par chale jayein to khatam ho jati hai. Jab team kehti hai "hamara workflow AI use karta hai", to iska matlab hota hai ke AI kuch named steps har dafa same tareeqe se karta hai, chahe keyboard par koi bhi ho. Sirf ye doosri soorat value mein barhti hai. Aur sirf yehi aisi ghalti kar sakti hai jo **barabar ghalat hoti rehti hai**.

Lesson ek kahani se shuru hota hai. Do teams ne same AI tool, same process aur same model contract review ke liye use kiya. **Pehli team** ne kaam step by step map kiya. AI ne clauses nikale, company ke playbook se departures flag kiye, aur **redline** draft kiya (redline woh marked-up version hota hai jo dikhata hai ke hum kya changes chahte hain). Phir ek lawyer ne har change approve kiya. Review ka time takreeban aadha ho gaya aur quality barqarar rahi. **Doosri team** ne poora process AI ko de diya. Draft acha tha, to unhon ne low-risk clauses AI ko khud approve karne diye. Ek mahine mein ek approved clause ne aisi obligation bana di jo kisi ne pakri nahi, aur tool wapas le liya gaya.

Dono teams ka farq tool mein nahi tha. Farq ye tha ke **kaun se steps AI ko diye gaye**. Is ke saath ek aur galti hai jo hum sab karte hain: ek disappointing jawab aaye to hum kehte hain "tool ye kar hi nahi sakta" ya randomly words badalte rehte hain. Ye dono ek hi ghalti hain, bas ulti directions mein. Dusri team ne **achhe output** ko dekh kar maan liya ke step safe hai. Hum **bure output** ko dekh kar maan lete hain ke task impossible hai. Isi liye course ka sab se bara usool ye hai: **"The output is not the verdict."** Output se faisla mat karo. Faisla in chaar cheezon se karo: kaun sa step hai, ghalti ki cost kya hai, jawab-deh kaun hai, aur problem kab shuru hui.

## Kahani 2: Pehle kaam ko design karo (Design stage)

**Design** ka matlab hai tool lagane se *pehle* ye tay karna ke kaam ki asal zaroorat kya hai aur kaun se numbers compute karne hain.

Asal kaam aksar saaf brief se shuru nahi hota. Wo 40 page ke document, adhoori emails ya meeting mein kahi hui kisi baat se shuru hota hai. Isay pehle **requirements** mein badalna parta hai, aur requirements teen cheezein hon: **specific, traceable aur testable**. AI is kaam mein bohat acha hai.

Misaal ke liye source ek **RFP** leta hai. RFP (request for proposal) woh document hota hai jo khareedar suppliers ko bhejta hai ke wo bid karein. AI se **summary mat maango, table maango**. Summary sirf batati hai ke document kya kehta hai, jabke table aisi rows deta hai jin par log kaam kar sakte hain. Table mein har requirement ka short label ho, wo section jahan se aayi (taake jo banda meeting mein nahi tha wo bhi check kar sake), ye ke kya thread pehle se isay answer karta hai, aur ye ke kya wo itni ambiguous hai ke clarifying question chahiye.

Kabhi kabhi document hota hi nahi, sirf ek jumla hota hai, jaise "hamein better reporting chahiye". Ye requirement nahi hai, kyunke koi isay bana nahi sakta aur koi baad mein bata nahi sakta ke wo poori hui ya nahi. Isay theek karne ke liye **task definition** banate hain: business need ko **paanch settled jawabon** mein badalna. Pehla, **what** produce hoga. Doosra, **for whom**. Teesra, **how often**. Chautha, **from what data**. Paanchwan, **in what format**. Jo jawab abhi missing hai wo aisa clarifying question hai jo aap kisi ke qarz-dar hain. Wo blank nahi jo model apni marzi se bhare, kyunke model jo slot aap nahi bharte unhein sab se mamooli (likely-looking) default se bhar deta hai.

Phir list ko **attack** karte hain. Extraction sirf wo dhoondti hai jo *likha* hai, wo nahi jo *matlab* tha. Jo requirements bid haraate hain wo aksar plainly nahi likhi hotin. Wo kisi chhoti clause mein, scoring rule ke peeche, ya aisi jumle mein hoti hain jise do log alag parhte hain. Is liye AI se poochte hain: kaun si ambiguous hai, kaun si ko do log alag samjhenge, aur kaun si sirf indirectly implied hai. Isse checking output stage se requirements stage mein aa jati hai, jahan wo bohat sasti hai: ek clarifying question ka kharcha, poora kaam bekar hone ke muqable.

Ambiguity pakarne ka ek asaan test hai: **"kya main is ka check likh sakta hoon?"** Agar nahi bata sakte ke kaun sa evidence prove karega ke requirement poori hui, to wo abhi decide hi nahi hui. Misaal: "report month end ke baad *promptly* deliver ho". Do din aur do hafte, dono kisi ke liye prompt hain, to do teams do alag process bana lengi aur dono samjhengi ke unhein yahi kaha gaya tha.

## Kahani 3: Numbers aur planning

Ab planning mein do alag kism ke kaam mix hote hain. **Synthesis** ka matlab hai considerations jama kar ke options banana. AI isme acha hai. Doosra kaam **calculation** hai, aur masla ye nahi ke AI add nahi kar sakta. Masla ye hai ke aap page dekh kar bata nahi sakte ke usne number calculate kiya ya sirf likh diya, kyunke dono ek jaise dikhte hain.

Isi liye rule consequence par based hai, ability par nahi: **"If a result matters, compute it. Never write it."** Computation ke liye **code execution** use hota hai. Iska matlab hai ke assistant ek chhota code likhta hai, chalata hai, aur batata hai ke kya compute hua. Source ise **chautha output format** kehta hai (baqi teen: inline text, artifacts, structured data). Ek limit yaad rakhein: run exact hota hai, magar code assistant ne likha hai aur wo ghalat column utha sakta hai. Isliye check karein ke **kya compute hua**, sirf ye nahi ke compute hua.

Ek acha prompt pehle ticket data se growth aur per-analyst resolved tickets **compute** karwata hai, phir un figures se headcount **recommend** karwata hai, aur assumptions bhi maangta hai taake koi bina arithmetic dobara kiye recommendation se disagree kar sake.

Aisa recurring kaam hota hai to wo ek **Project** mein jata hai. **Project** ek kism ke kaam ka saved workspace hota hai. Uske andar teen cheezein rehti hain. **Knowledge base** woh files hain jo Project parh sakta hai (jaise purane winning proposals). **Standing instruction** woh rule hai jo har run par lagta hai (jaise extraction ka format). **Skill** ek saved procedure hai jo assistant har dafa same tareeqe se follow karta hai (jaise formatting ki procedure). Skill account level par hoti hai, is liye har Project mein kaam karti hai aur ek edit sab jagah apply ho jata hai.

## Kahani 4: Kya AI ye step le sakta hai? (Window test)

Ek operations lead ne ek hi request mein data analysis, growth trend aur headcount recommendation maangi. Jawab achha structured tha aur 3 analysts hire karne ko kaha. Magar team par do hafte pehle **hiring freeze** announce ho chuka tha. Ye freeze ek meeting mein decide hua tha, kisi dataset mein nahi tha. Trend analysis theek thi. Ghalti ek aise step ki thi jise zaroori input mil hi nahi sakta tha. Aur yahan ek khatarnaak baat hai: model **ruk nahi jata**. Wo gap ko usi cheez se bhar deta hai jaisa aise faisle "aam tor par hote hain", aur usi confidence ke saath jo us hisse mein tha jo usne waqai compute kiya.

Is liye course ek test deta hai: **window test**. Sawal ye hai: *"Kya main is step ki saari zaroorat model ke samne rakh sakta hoon? Nahi, to step mera hai."* Yahan "window" model ka **context** hai, yani jo kuch model is kaam ke liye dekh sakta hai: aap ka prompt, files, aur ab tak ki conversation. **Context window** us context ki hadd hai ke ek waqt mein kitna hold ho sakta hai. Isi hadd ki wajah se lamba session apni purani instructions kho deta hai (ye baat Diagnose wale hisse mein dobara aayegi).

Jo step aisi information par chalta hai jo aap supply nahi kar sakte (ya karna nahi chahte), use **judgment step** kehte hain, jaise risk appetite, hiring freeze, ya ye ke client ek aur delay maanega ya nahi. Ye insaan ke paas isliye rehte hain ke unke inputs available nahi, is liye nahi ke judgment muqaddas hai. Ye test un kaamon ko bhi pakarta hai jinhein log "human touch chahiye" kehte hain, jaise kisi purane client ko condolence note.

Research par bhi ye test lagta hai. Model ki knowledge ek tareekh par ruk jati hai, aur uske baad ki cheez window ke bahar hai. Isliye sawal ko pehle do hisson mein baantein. **Stable concept ya method** ho to model ki apni knowledge theek hai. **Kuch current, priced ya dated** ho to aisa external source maango jise aap khud khol sakein, yani jawab **aur link**. Rule: *"For anything current, ask for a source you can open. Never a confident answer."*

## Kahani 5: Map banana (Delegation map)

Ab asli kaam: **delegation map** banana. Delegation map poora workflow hota hai, step by step, har step ke saamne **owner aur wajah** likhi hui.

Har step par **teen alag faisle** hote hain, aur inhein mix karne se aise map bante hain jo reasonable lagte hain magar ghalat hote hain. Pehla faisla **Eligibility** hai: kya AI is ko chhoo bhi sakta hai? Iske do gates hain. **Data gate** poochta hai ke kya ye data is tool mein jaiz hai (ye Governance course ka sawal hai). **Input gate** wohi window test hai. Kisi bhi gate par "nahi" aa jaye to baat wahin khatam, chahe step kitna mechanical lage. Doosra faisla **Ownership** hai: step ka owner kaun hoga? Teesra faisla **Implementation** hai: kaun si cheez wo step uthayegi? Ye sab se aakhir mein tay hota hai, aur sirf unn steps ke liye jo pehle do faisle paas kar chuke hon.

Ownership **teen criteria** se tay hota hai, sirf yehi teen:

**Pehla: Reversibility.** Agar AI ghalti kare to kya hum use undo kar sakte hain? Draft dobara likha ja sakta hai, magar bheji hui email unsend nahi hoti. Jo undo ho sakta hai usay delegate karna aasan hai.

**Doosra: Stakes.** Ghalti ki cost kya hai, **bure case mein**? Average ya "aam tor par" nahi. Galat label ek minute zaya karta hai, magar galat penalty figure ki cost poori penalty hai.

**Teesra: Accountability.** Har step ka koi na koi jawab-deh hota hai, isliye sirf "koi jawab-deh hai" kehna kafi nahi. Asal sawal ye hai ke **kya ye step khud wo faisla hai jiska banda jawab deta hai, ya ye ek input hai jise koi aage judge karta hai?** Agar input hai jise koi judge karta hai, to step delegate ho sakta hai, kyunke accountability judging par hai. Agar step khud faisla hai, to delegate nahi ho sakta. Accountability kabhi machine par nahi jati, kyunke machine se poocha nahi ja sakta.

In teen criteria ke bare mein teen cheezein yaad rakhein. Ye **score nahi, teen sawal** hain, aur aam tor par ek criterion step ka faisla karta hai aur baaki do us se agree karte hain. Aap ko us ek ka naam likhna chahiye, taake koi aur check kar sake. Agar teeno mein ikhtilaf ho to **sab se strict wala jeetta hai**. Aur "AI ne is par pehle achha kaam kiya" criterion **nahi** hai.

In criteria se har step **teen classes** mein se ek mein jata hai. **AI-appropriate** step AI own kar sakta hai, kyunke wo undo ho sakta hai aur koi uska nateeja judge karta hai. **Human-retained** step insaan poori tarah own karta hai. **Collaborative** step mein AI banata hai aur ek **naam wala insaan** judge karta hai. Jis lamhe koi judge nahi karta, wo step collaborative nahi rehta.

Misaal: contract review mein clauses nikalna AI ka hai. Redline draft collaborative hai. Har change approve karna aur sign and send karna insaan ke hain. Penalty exposure ka calculation bhi AI karta hai, lekin us ki wajah ye nahi ke wo arithmetic hai. Wajah ye hai ke wo reversible hai aur agle hi step mein ek insaan ke saamne aata hai.

Teesre faisle **Implementation** mein paanch carriers hain. Fixed procedure ko **Skill** uthati hai. Wo rules aur reference jo step ko hamesha chahiye **Project knowledge** mein jate hain. Jis calculation par output depend karta hai wo **Code execution** karta hai. Har output par lagne wali constraint **Standing instruction** mein jati hai. Aur jo step insaan ke paas hai uske liye **Named review gate** chahiye: ek banda, ek lamha, aur ek cheez jo wo check karta hai. Sirf "human" likhna kafi nahi. Zaroori baat: "isay compute karna hai" Implementation ki baat hai, ye AI ko step dene ki wajah nahi. Isi ghalti se high-stakes calculation bina review ke reh jati hai.

## Kahani 6: Map kaise ghalat hota hai

Dusri team bekar nahi thi. Unhon ne hafton tak AI ko achhi redlines draft karte dekha, phir aasan clauses approve karne ko de diye. Ye evidence par ek reasonable reaction lagta hai, aur yehi sab se aam tareeqa hai jis se workflow mein aisa risk aa jata hai jo kisi ne chuna nahi. Isko **over-delegation** kehte hain: AI ko step ke risk se zyada de dena.

Is ke teen roop hain. **Halo delegation**: pichla step achha gaya, isliye agla bhi AI ko de diya. Competence asli thi, magar wo kisi aur step ki thi. Yaad rakhein: *"Drafting quality is evidence about the draft. It is not evidence about the decision."* **Unstaffed gate**: collaborative step ka review ab sirf naam ka reh gaya hai. Reviewer busy hai, queue lambi hai, drafts do mahine se achhe hain, to review pehle glance bana aur phir sirf click. Kisi ne kuch decide nahi kiya aur map badla nahi, magar step ab automated hai. Map ye nahi batata kyunke map wo likhta hai jo **design** kiya tha, wo nahi jo **chal raha hai**. **Mapping the tool instead of the work**: team apni pasandeeda feature ke mutabiq workflow banati hai (ek acha Skill bana to workflow mein us jaisa step add kar liya). Ye teeno mein sab se mushkil se nazar aata hai.

Isliye check ka order ye hai: pehle bina tools ke kaam map karo, phir har step ko alag classify karo, aur phir har collaborative step par poocho: **kaun review kar raha hai aur kab?**

## Kahani 7: Map ko sach kaise rakhein

Map ek dafa likha jata hai aur phir dheere dheere ghalat ho jata hai, kisi ke badle bina, kyunke workflow uske neeche se hil jata hai. Koi step add hua, koi reviewer ka role badla, volume doguna ho gaya aur jo gate 20 cases par chalta tha wo 50 par fail ho gaya. Is course ke teen controls isi tarah decay hote hain, aur teeno mein fail hone ke waqt **koi signal nahi aata**: review gate (glance phir click), standing instruction (output dheere dheere rule se hat jata hai), aur map khud (wo workflow batata hai jo ab koi nahi chalata).

Ek hi jawab hai: **scheduled read**, yani tay shuda tareekh par map ka review. Map ko do cheezein chahiye. Pehli, ek **map owner**: ek naam wala banda (team nahi), jo kaam nahi karta magar is baat ka jawab-deh hai ke map abhi bhi haqeeqat batata hai. Doosri, ek **review date**, aam tor par quarterly, aur agar volume, staffing ya legal position badle to jaldi.

Review chaar sawalon ka hota hai aur takreeban 20 minute leta hai. Pehla: kya koi step add ya remove hua jo map par nahi? Doosra: har collaborative step ko **pichle hafte** kis ne review kiya aur kitni der? Agar koi nahi bata sakta to step automated hai. Teesra: kya volume ya stakes badle? Chautha: kya har configuration abhi current hai (Skills, knowledge sources, standing instructions)? Doosra sawaal asal masle pakarta hai, kyunke wo policy ke baare mein nahi, balkay *pichle hafte* ke baare mein hai.

## Kahani 8: Banana (Build)

Ab jab map ban gaya, to cheez banane ka tareeqa kya hai? AI aap ka **design partner** hai, vending machine nahi. Wo sirf us par react karta hai jo aap uske saamne rakhte hain. Solution maangne se nahi milta, **loop** chalane se milta hai, jis ke chaar steps hain. **Ideate**: options banana. **Prototype**: ek option ko itna concrete banana ke us par reaction de sakein. **Feedback**: dekhna kya ghalat hai, jo pehle se pata nahi tha. **Refine**: usay theek karna. Phir doosra round. Ye loop ek Project ke andar chalayein, taake background aur purane faisle stable rahein.

Source ka example ek business analytics team ka hai jis ne ek **artifact** banwaya. Artifact ek chhota working web page hota hai jo assistant chat ke andar banata hai. **Cycle 1** mein 5 metrics ke charts ban gaye, aasan tha. **Cycle 2** mein date filter aur totals row maangi. Filter chala, magar totals ghalat the, aur itne ghalat nahi ke nazar aayein, kyunke figures sahi size ke aur sahi format mein the. Ek analyst ne pakra kyunke use ek number ka andaza tha. Wajah wohi hai jo pehle bataya: totals **likhe** gaye the, compute nahi hue. Ye **feature problem** tha, behtar description se hal nahi hota. **Cycle 3** mein color aur print layout maange, aur wo pehli koshish mein chal gaya. Ye **description problem** tha. In dono mein farq pehchanna hi asal hunar hai.

Ek aur baat. Ek chhota internal tool 6 mahine baad aisa ban gaya ke 3 departments har Monday use kar rahe hain aur ek department uske numbers board report mein dal raha hai. Ab ye ek alag cheez hai jo kisi ne decide nahi ki. **Escalation signal** ka matlab hai wo lamha jab koi tool prompt-and-iterate se bahar nikal jaye. Jab doosre log us par infrastructure ki tarah depend karne lagein, to usay ye cheezein chahiye jo pehle nahi thin: uptime, access control, kisi ko bulane ka tareeqa, aur ye guarantee ke aaj bhi wohi karta hai jo March mein karta tha. Ye developer ya architect ka kaam hai. Escalate karna **sahi jawab** hai, nakami nahi. Nakami ye hai ke aap prompt se chalate rahein jabke doosre depend karne lagein.

Do signals aise hain jo ek jaise lagte hain. **"Doosre log ab is par depend karte hain"** ka matlab hai ye infrastructure hai aur engineering chahiye. **"Maine ye teen baar ek hi tareeqe se hal kiya"** ka matlab hai tareeqa stable ho gaya hai aur isay worker mein manufacture kiya ja sakta hai (From One-Off to Worker course). Pehla batata hai kaun exposed hai, doosra batata hai ke tareeqa badalna band ho gaya.

## Kahani 9: Kharabi aaye to kaise dhoondein (Diagnose)

Output kharab aaye to log ya haar maan lete hain ya random cheezein badalte hain. Dono ek hi sawal skip karte hain jo problem ko chhota kar deta hai: **symptom pehli baar kab aaya?** Timing free information hai jo aap ke paas pehle se hai. Yaad rakhein: timing sirf ye batati hai ke **pehle kahan dekhna hai**, ye nahi ke wajah kya hai.

Chaar wajohat hain, aur chaaron page par ek jaise dikhte hain:

**Pehli: Under-specification.** Symptom pehle hi jawab se ghalat tha. Matlab prompt ne wo cheez carry hi nahi ki jo step ko chahiye thi. Test: prompt dobara parhein, kya missing cheez waqai us mein hai? Fix: jo choota use add karein. Ye sab se aam wajah hai aur sab se sasta fix.

**Doosri: Context overload.** Shuru mein theek chalta tha, phir kharab hota gaya. Matlab conversation context window se lambi ho gayi, isliye purana text chhota ya gir gaya aur early instructions kamzor ho gayin. Test: fresh session mein wohi instruction dohrayein, kya ab theek chalta hai? Fix: restart ya summary. Behtar prompt yahan kaam nahi karta.

**Teesri: Wrong feature or model.** Ek hi qism ki ghalti baar baar aati hai. Numbers thode ghalat hain to calculation prose mein maangi gayi thi. Kaam gehra tha magar shallow nikla to **tier** speed ke liye chuna gaya tha. Tier model ka version hota hai, tez aur sasta se le kar slower aur zyada capable tak. Test: wohi step ek baar sahi feature ya mazboot tier par chalayein. Fix: feature ya tier badalna.

**Chauthi: Stale configuration.** "Pehle theek chalta tha, ab nahi." Koi saved instruction, file ya Skill purani ho gayi. Ye sab se khatarnaak hai kyunke **silent** hai: koi error ya warning nahi aati. Pichle quarter ke figures knowledge base mein pare hain aur is quarter ki report unhein quote karti hai, bilkul perfect format mein. Model ko pata hi nahi ke jo aap ne diya wo purana hai. Fix: configuration ki maintenance. Ye unstaffed gate ka jorha hai: dono mein ek control sahi set hota hai aur sab ke maan lene ke dauran decay ho jata hai.

Ab in sab ko kis **order** mein check karein? **Diagnostic sequence** paanch steps ki hai, aur **sasta pehle**. **Step 1** mein prompt dobara parhein, uske paanch hisson ke against: role, context, task, constraints, aur format. Ye slot by slot isliye kyunke likhne wale ko prompt theek lagta hai, jo kami hai wo uske dimagh mein hoti hai. **Step 2** mein conversation ki lambai dekhein. **Step 3** mein feature aur model dekhein. **Step 4** mein dekhein ke configuration current hai ya nahi. **Step 5** mein, aur sirf ab, ye poochein ke kya task fit hi hai. Log is ko ulta chalate hain: seedha sab se mazboot model ya "task impossible" par jump karte hain.

Step 5 kabhi kabhi sahi bhi hota hai. **Expectation mismatch** ka matlab hai aisa task jo tool kar hi nahi sakta, jaise "agle quarter ki exact sales figure batao". Isko koi prompt, restart ya feature theek nahi karta. Fix task ko badalna hai: ek range maangein assumptions ke saath, ya aisa model jis ke drivers aap adjust kar ke dobara chala saken. Magar ye step 5 isi liye hai ke pehle 4 cheaper wajohat rule-out hon.

## Kahani 10: Fix ko hamesha ke liye rakho (Persist)

Har disappointing output setup ke baare mein kuch batata hai, magar zyada tar fix haath se kar diya jata hai aur wo information zaya ho jati hai. Pehla kadam: **reaction ko instruction mein badlo**. Reaction sirf feel batati hai ("too generic", "not quite right"). Instruction batati hai ke kya badalna hai. Ek sawal ye jump karwata hai: *"sahi hone ke liye kya present hona chahiye tha, aur setup ka konsa hissa (lever) isay control karta hai?"* Lever teen ho sakte hain: prompt, standing instruction, ya knowledge. Agar lever ka naam nahi le sakte, to aap ki critique abhi bhi sirf reaction hai aur agla attempt ek guess hoga.

Phir doosra masla: fix mil gaya magar chat mein reh gaya. Source ka analyst har mahine chat mein likhta tha "cancelled orders exclude karo", aur wo kaam karta tha. Magar jab wo do hafte chhutti par gaya aur colleague ne report chalayi, to cancelled orders shaamil ho kar numbers bahar chale gaye. Fix tha, magar aisi jagah jahan sirf ek banda dhoondh sakta tha.

Is liye **promotion** hai: fix ko chat se nikal kar configuration mein dalna taake wo hamesha lage. Test: *"Kya ye correction dobara chahiye hogi, mujhe ya kisi aur ko?"* Agar haan, to configuration mein jaye. Aur kahan? Teen ghar hain: **Rule** (aisi limit jo hamesha lagti hai) standing instruction mein jata hai, jaise "pehli line mein target segment zaroor likho". **Reference** (aisa material jo kaam ko parhna padta hai) knowledge base mein jata hai, jaise brand voice guide ya current product list. **Procedure** (steps ka ek sequence) Skill mein jata hai, jaise "weekly report is exact format mein is order mein banao". Galat ghar mein daalne se fix tikta nahi: procedure ko ek line ki instruction bana do to order kho jata hai, aur reference ko standing instruction mein thoon do to har prompt bhari ho jata hai chahe is run ko uski zaroorat ho ya na ho. Aur "memory" iska badal nahi, kyunke wo per-user hai (colleague ko nahi milti) aur best-effort hai (aap use point ya hand over nahi kar sakte). Configuration shared aur parhne ke qabil hai.

## Kahani 11: Chhote kharche dhoondo (Friction)

**Friction** woh chhota, bar bar hone wala kharcha hai jise aap ne dekhna chhor diya. Do minute ka reformat kisi ko nahi khatakta, magar saal mein 50 dafa hota hai. Teen signals batate hain ke friction mauzood hai jo configuration se hata sakte hain. **Repetition**: aap har run mein wohi cheez paste ya type karte hain (fix: saved context ya standing instruction). **Correction**: aap har output mein wohi flaw theek karte hain (fix: configuration badlo ke wo aaye hi nahi). **Variance**: alag alag log wohi kaam karte hain to alag nateeje aate hain (fix: shared Skill ya knowledge base). Variance wohi hai jo log sab se zyada miss karte hain, kyunke kisi ek banday ko mehsoos nahi hoti. Wo sirf reviewer ke paas dikhti hai jo teeno ke updates ko ek voice mein likhta hai.

Friction hatane ke do moves hain, **is order mein**. Pehla **consolidate**: steps ko ek saath chalana, taake teen prompts jo har dafa wohi background maangte hain ek ban jayein. Doosra **promote**: repeated pattern ko configuration mein daalna. Consolidate pehle isliye ke jo step merge hone wala hai usay promote karna zaya mehnat hai.

## Kahani 12: Improvement ko naapna (Measure)

Jo improvement naapi nahi gayi, usay justify karna mushkil hai aur barqarar rakhna mushkil tar. Source ka example: reporting ka kaam 45 minute se 25 minute par aaya. Ye jumla tabhi kaha ja sakta hai jab kisi ne badalne se **pehle** naapa ho. Ye naap **baseline** kehlati hai. Isme teen numbers hote hain: kitna time laga, kitne revision rounds lage, aur kitne manual steps kiye. Baad mein baseline banayi nahi ja sakti, kyunke purane tareeqe ka aap ka andaza aap ko flatter karega.

Sirf time save karna aksar sahi metric nahi hota. Metric wo chunein jo is wajah se match kare ke workflow mahatvapurn kyun tha. **Internal draft** ke liye **time**, kyunke speed ahem hai aur chhoti ghalti sasti hai. **Customer ko jane wali report** ke liye **consistency**, kyunke alag alag formats bharosa torte hain. **Compliance ya finance output** ke liye **accuracy**, kyunke ek ghalat figure ek ghante ki bachat se mehnga hai. **Kai logon ke kiye hue kaam** ke liye **variance**, kyunke kharcha logon ke beech mein hota hai. Metric pehle se chun lein to ye bhi pata chalta hai ke kab rukna hai.

Phir **parallel run**: purane aur naye workflow ko 2 se 3 cycles saath chalana. Isme duplicate kaam hota hai, lekin teen faide milte hain: naya tareeqa behtar hone ka evidence, agar na ho to ek chalta hua fallback, aur un logon ki razamandi jin ka kaam badla (kyunke "hum aap ka kaam badal rahe hain" ki jagah "humne dono chalaye, ye nateeja hai" kehna aasan hota hai).

Aur budget review ke liye cost batani hoti hai. **Cost** = AI tool ka kharcha + insaani waqt jo gates mein bacha hua hai. **Saving** = baseline x kitni dafa chalta hai x kitne log chalate hain. Misaal: 20 minute hafta x 3 analysts takreeban 50 ghante saal. Phir wo risk bhi batayein jo aap ke gates ke baad bhi bacha hai, kyunke jo business case risk chhupata hai usay phir koi nahi manta.

## Kahani 13: Bura output bahar nikal jaye to (Incident path)

Ab tak jo kuch kiya wo bure output ke bahar jane ka chance **kam** karta hai, khatam nahi. Kisi busy Friday ko gate skip ho jata hai, ya configuration do reviews ke beech stale ho jati hai. Aur us ghante mein design judge hota hai, map nahi. Zyada tar teams ke paas us ghante ka koi plan nahi hota, to jawab improvise hota hai, sust aur defensive.

Workflow ka designer **chaar cheezein pehle se tay** karta hai. **Pehla: Stop.** Is workflow ko sab se tezi se kaun rok sakta hai, aur kya use permission chahiye? Agar sachha jawab hai "hamein us se poochna parega jis ne isay set kiya tha", to pehle ye theek karein. **Doosra: Scope.** Sirf ye nahi ke ye ek output ghalat tha, balkay **kitne outputs affect hue aur kahan gaye?** Stale configuration ek bura result nahi deti, jis din se wo stale hui us ke baad ka har result kharab hota hai. **Teesra: Tell.** Kis ko batana hai (customer, internal owner, risk ya compliance team) aur kab tak? Ye pehle tay karein, kyunke us waqt der karne ka dabao bohat zyada hota hai aur late disclosure bohat mehnga parta hai. **Chautha: Map change.** Har incident design ke baare mein kuch batata hai. Chaar wajohat mein se kaun si thi? Kya step ghalat classify hua, ya theek classify hua magar gate staff nahi tha? Map mein tareekh ke saath tabdeeli likhein taake wo us hafte se zyada tike jab sab dhyan de rahe the. Faisle 1 aur 4 workflow designer ke hain aur design ke waqt hone chahiye, warna kabhi nahi.

## Kahani 14: Doosron ko kaise batayein (Communicate)

Aakhir mein AI workflow ko un logon ko batana parta hai jinhon ne use banaya nahi: manager, client, risk team. Bharosa tab milta hai jab aap sach batate hain, yani limits utni saaf batayein jitni value. Teen jumle overstate karte hain: **"Fully automated"** (lagbhag kabhi sach nahi aur pehli visible ghalti public mein expose kar deti hai), **"AI handles X"** (jumle se human gate ghayab ho jata hai aur sunne wala samajhta hai koi gate hai hi nahi), aur **"It's basically aood as a person at Y"** (aisa maiyar jo tool kabhi na kabhi miss karega, us ke saamne jise aap ki baat yaad hai).

Hal har dafa wohi hai: **batayein tool kya karta hai, phir human checkpoint ka naam lein.** Sirf ek extra jumla lagta hai magar wo aisa daawa banata hai jo aap defend kar sakte hain. Jab audience ye faisla kar rahi ho ke workflow par bharosa karein ya nahi, to ek teesra jumla bhi add karein: **batayein ke wo kya refuse karta hai**, yani wo cases jo wo hand over karta hai (unclear clause, ghair mamooli contract, playbook se bahar ki request). Ye list batati hai ke boundary pehle se design ki gayi thi, kisi incident mein dhoondi nahi gayi.

Wohi workflow teen audiences ko teen tarah se bataya jata hai. **Legal lead** ko mechanism aur failure modes chahiye ("clauses nikalta hai, playbook se departures mark karta hai, pehli redline likhta hai, approve karna aap ka kaam hai, aur jo implied obligation likhi nahi hoti wo miss ho sakti hai"). **Practice executive** ko outcome aur oversight chahiye ("turnaround do din se takreeban aadha din, aur har change par lawyer sign off karta hai"). **Client ki risk team** ko control chahiye ("drafting AI-assisted hai, har term ek qualified lawyer approve karta hai, bina sign-off ke kuch nahi jata"). Teeno mein gate shaamil hai. Is liye ye zaroori usool hai: **jab human checkpoints saaf batayein jayein, stakeholders AI workflow par zyada bharosa karte hain, kam nahi.**

## Poori kahani ek line mein

Pehle batayein kaam kya hai (Design), phir har step ko teen criteria se owner dein (Map), loop se banayein (Build), kharabi ho to timing se dhoondein (Diagnose), fix ko configuration mein rakhein (Persist), aur doosron ko sach batayein ke kya karta hai aur gate kahan hai (Communicate).

> **The output is not the verdict. Judge the step by what it costs and who answers for it, and judge a failure by when it started.**
Neeche sawal wese hi bane hain jaise sir poochte hain: **"X kya hai?"**, **"kitni types/options hain?"**, **"kyun?"**, **"farq kya hai?"** aur scenario. Har jawab lesson ke mutabiq hai, aur pehle chhota jawab hai, phir wajah.

Ek note: lesson mein ye 6 stages ek hi table mein aate hain, aur course ke 6 Parts bhi isi order mein chalte hain. Design = Part 1, Map = Part 2, Build = Part 3, Diagnose = Part 4, Persist = Part 5, Communicate = Part 6. Ye mapping meri clarification hai.

# Section A: "X kya hai?" (Pehle har stage)

**Q1. Design kya hai?**
Design ka matlab hai tool lagane se *pehle* kaam ko design karna: asal requirements kya hain aur kaun se numbers compute karne hain. Is mein teen kaam aate hain: messy document ko requirements mein badalna, un par "attack" karna (kaun si ambiguous hai), aur numbers ko likhne ke bajaye compute karwana. Misaal: "we need better reporting" requirement nahi, isay task definition ke 5 jawabon mein badalna design hai.

**Q2. Map kya hai?**
Map (delegation map) poora workflow step by step hota hai, jis mein har step ka **owner** (AI, insaan, ya collaborative) aur **wajah** likhi hoti hai. Har step ko teen criteria se parkha jata hai: reversibility, stakes, accountability. Misaal: contract review mein "extract clauses" AI ka, "approve each change" insaan ka.

**Q3. Build kya hai?**
Build ka matlab hai solution ko ek prompt se nahi, balkay ek **loop** se banana: ideate, prototype, feedback, refine. Aur ye pehchanna ke kab cheez prompt-and-iterate se bahar nikal gayi (escalation signal). Misaal: dashboard artifact jo 3 cycles mein bana.

**Q4. Diagnose kya hai?**
Diagnose ka matlab hai bure output par haar maanne ya random changes karne ke bajaye **symptom ki timing** se wajah dhoondna. Chaar wajohat hain aur paanch steps ka sequence jo sasta pehle chalta hai. Pehla sawal hamesha: "symptom kab aaya?"

**Q5. Persist kya hai?**
Persist ka matlab hai jo fix aap ne dhoondha usay chat mein chhorne ke bajaye **configuration mein daalna** taake wo hamesha lage. Source isay **promotion** kehta hai. Test: "kya ye correction dobara chahiye hogi?" Agar haan, to promote karo. Is stage mein ye cheezein bhi aati hain: reaction ko instruction banana, fix ka sahi ghar (rule/reference/procedure), friction dhoondna, aur improvement naapna.

**Q6. Communicate kya hai?**
Communicate ka matlab hai doosron (manager, client, risk team) ko sach batana ke AI workflow kya karta hai: **value bhi aur limits bhi**, aur **human gate ka naam** lena. Is ke saath ye bhi aata hai ke bura output bahar nikal jaye to kya karna hai (incident path), jo pehle se tay hota hai.

# Section B: "Kitni types, kitne options?" (Count wale sawal)

**Q7. Course ke kitne stages hain, naam aur har ka deciding sawal?**
**6 stages**:
1. Design: requirements kya hain, kaun se numbers compute hon?
2. Map: undo ho sakta hai, error ki cost, jawab kaun deta hai?
3. Build: kya ye abhi bhi prompt-and-iterate mein fit hai?
4. Diagnose: symptom kab aaya?
5. Persist: ye fix rule, reference ya procedure hai?
6. Communicate: ye kya karta hai, human gate kahan hai?

**Q8. Step ka owner tay karne ke criteria kitne hain?**
**3 criteria**, aur sirf yehi:
1. **Reversibility**: ghalti ho to undo ho sakta hai?
2. **Stakes**: bure case mein ghalti ki cost?
3. **Accountability**: kya ye step khud wo faisla hai jiska banda jawab deta hai, ya ek input jise koi judge karta hai?

Ye teen sawal hain, score nahi. Aam tor par ek criterion decide karta hai (uska naam likho), aur ikhtilaf ho to **strictest** jeetta hai. (Source ek 4-criterion version ka bhi zikr karta hai jo "creativity ya empathy chahiye?" jodta hai, magar wo poore use case ka sawal hai, step ownership ka nahi. Ownership ke liye teen hi hain.)

**Q9. Step ki kitni classes hain?**
**3 classes**: **AI-appropriate** (AI own kare), **Collaborative** (AI banaye, naam wala insaan judge kare), **Human-retained** (insaan poori tarah own kare).

**Q10. Har step par kitne faisle hote hain?**
**3 faisle**: **Eligibility** (kya AI chhoo sakta hai? is ke 2 gates hain: data gate aur window test), **Ownership** (3 criteria), **Implementation** (kaun si cheez kaam uthaye, sab se aakhir mein).

**Q11. Implementation ke kitne carriers hain?**
**5 carriers**: **Skill** (fixed procedure), **Project knowledge** (rules aur reference jo step ko hamesha chahiye), **Code execution** (calculation), **Standing instruction** (har output par constraint), **Named review gate** (insaani step: ek banda, ek lamha, ek cheez check karne ko).

**Q12. Map ki kitni ghaltiyan hain?**
**3 ghaltiyan**: **Halo delegation** (pichla step achha gaya to agla de diya), **Unstaffed gate** (review sirf naam ka reh gaya), **Mapping the tool instead of the work** (feature ke mutabiq workflow). Teeno ki chhatri **over-delegation** hai (step ke risk se zyada AI ko dena).

**Q13. Bure output ki kitni wajohat hain?**
**4 wajohat**: **Under-specification** (pehle jawab se ghalat), **Context overload** (shuru theek, phir kharab), **Wrong feature or model** (ek hi qism ki ghalti baar baar), **Stale configuration** ("pehle chalta tha"). Ek **paanchwa outcome** bhi hai, **expectation mismatch** (task hi aisa jo tool nahi kar sakta), magar ye cause nahi hai, aur sirf pehli 4 rule-out hone ke baad sahi hai.

**Q14. Diagnostic sequence mein kitne steps hain, aur order kya hai?**
**5 steps**, sasta pehle: (1) prompt dobara parho, uske 5 hisson ke against: role, context, task, constraints, format. (2) conversation ki lambai. (3) feature aur model. (4) configuration current hai? (5) sirf ab: kya task fit hai?

**Q15. Build loop mein kitne steps hain?**
**4 steps**: **Ideate** (options banao), **Prototype** (itna concrete ke reaction de sako), **Feedback** (jo pehle pata nahi tha wo dikhna), **Refine** (theek karo). Phir dobara.

**Q16. Fix ke kitne "ghar" hain?**
**3 ghar**: **Rule** to **Standing instruction**, **Reference** to **Knowledge base**, **Procedure** to **Skill**. Rule hamesha lagne wali limit hai, reference wo material hai jo kaam ko parhna hai, procedure steps ka sequence hai.

**Q17. Friction ke kitne signals aur moves hain?**
**3 signals**: **Repetition** (wohi paste/type har run), **Correction** (wohi flaw har output mein theek karna), **Variance** (alag log, alag result). **2 moves**, is order mein: **Consolidate** (steps milao), phir **Promote** (pattern configuration mein).

**Q18. Metrics kitne hain aur kab kaun sa?**
**4 metrics**: internal draft ke liye **time**, customer report ke liye **consistency**, compliance/finance ke liye **accuracy**, kai logon ke kaam ke liye **variance**.

**Q19. Bura output nikal jaye to kitne faisle pehle se tay hote hain?**
**4 faisle**: **Stop** (kaun rok sakta hai, bina permission ke?), **Scope** (kitne outputs affect hue, kahan gaye?), **Tell** (kis ko, kab tak?), **Map change** (kaun si cause thi, tareekh ke saath tabdeeli). Faisle 1 aur 4 designer ke hain, design time par.

**Q20. Communicate mein kitne galat jumle aur kitni audiences?**
**3 galat jumle**: "Fully automated", "AI handles X", "It's basically as good as a person at Y". **3 audiences**: legal lead (mechanism aur failure modes), practice executive (outcome aur oversight), client ki risk team (control). Teeno ke versions mein gate shaamil hai.

**Q21. Task definition ke kitne jawab hain?**
**5 jawab**: **what** produce hoga, **for whom**, **how often**, **from what data**, **in what format**.

**Q22. Output ke kitne formats hain?**
**4 formats**: inline text, artifacts, structured data, aur **code-executed** (code execution ka result).

**Q23. Escalation ke kitne signals hain?**
**2 signals**: "doosre log ab is par depend karte hain" to developer ya architect. "Maine ye teen baar ek hi tareeqe se hal kiya" to From One-Off to Worker course.

**Q24. Map review ke kitne sawal hain?**
**4 sawal** (takreeban 20 minute): koi step add/remove hua? Har collaborative step ko pichle hafte kis ne review kiya aur kitni der? Volume ya stakes badle? Har configuration current hai?

**Q25. Eligibility ke gates aur research ki qismein kitni hain?**
**2 gates**: **Data gate** (kya ye data tool mein jaiz hai?) aur **Input gate / window test** (kya saari zaroorat window mein rakh sakte ho?). Research ke sawal **2 qism** ke: stable concept (model ki knowledge theek) aur current/priced/dated (source maango jo khol sako).

# Section C: "Kyun?" wale sawal

**Q26. Design pehle kyun karte hain, seedha tool kyun nahi lagate?**
Kyunke asal kaam aksar messy hota hai (40 page ka document, adhoori emails). Agar requirements saaf na hon to do teams do alag cheezein bana lengi. Ek unclear requirement design ke waqt pakri jaye to ek clarifying question ka kharcha hai, baad mein pakri jaye to poora kaam bekar.

**Q27. Numbers compute kyun karte hain, likhwate kyun nahi?**
Masla ye nahi ke AI add nahi kar sakta. Masla ye hai ke likha hua aur calculate kiya hua number page par **ek jaise dikhte hain**, aur aap bata nahi sakte ke kaun sa kaun sa hai. Isliye rule hai: *agar result matter karta hai to compute karo, kabhi likhwao mat.*

**Q28. Window test kyun?**
Kyunke jab input model ko mil hi nahi sakta (jaise hiring freeze jo meeting mein tay hua), to model **rukta nahi**, wo aam tor par aise faisle jaise hote hain us se gap bharta hai, aur usi confidence se jo us hisse mein tha jo usne waqai compute kiya. Isliye step jis ki zaroorat window mein na aaye wo insaan ka rehta hai.

**Q29. Accountability kabhi machine par kyun nahi jati?**
Kyunke machine se poocha nahi ja sakta. Aur har step ka koi na koi jawab-deh hota hai, isliye asal sawal ye hai ke *kya ye step khud wo faisla hai jiska banda jawab deta hai*, ya ek input jise koi aage judge karta hai.

**Q30. Persist kyun karte hain?**
Kyunke fix chat mein reh jaye to agli baar (aap ya koi aur) wohi mehnat dobara karega. Source ka analyst har mahine chat mein likhta tha "cancelled orders exclude karo". Wo chhutti par gaya to colleague ki report mein cancelled orders aa gaye. Fix mauzood tha, bas aisi jagah tha jahan sirf ek banda dhoondh sakta tha.

**Q31. Memory persist ka badal kyun nahi?**
Memory **per-user** hoti hai (colleague ko nahi milti) aur **best-effort** hoti hai (aap point, read ya hand over nahi kar sakte). Configuration shared aur parhne ke qabil hai.

**Q32. Baseline pehle kyun naapte hain?**
Kyunke baad mein baseline banayi nahi ja sakti, purane tareeqe ka aap ka andaza aap ko flatter karega. Baseline ke bina "45 se 25 minute" jaisa jumla sirf ek yaqeen hai, saboot nahi.

**Q33. Parallel run kyun?**
Isme duplicate kaam hota hai, magar 3 faide milte hain: naya tareeqa behtar hone ka **evidence**, agar na ho to ek chalta hua **fallback**, aur un logon ki **razamandi** jin ka kaam badla. Ye teesra sab se zaroori hai, kyunke "hum aap ka kaam badal rahe hain" ki jagah "humne dono chalaye, ye nateeja hai" kehna aasan hota hai.

**Q34. Human gate kyun batate hain, isse tool kam impressive nahi lagta?**
Source ke mutabiq ulta hota hai: gate saaf batane se stakeholders ka bharosa **barhta** hai. "AI karta hai" aur "AI ghalat ho to kya hota hai" ke beech ka khali gap wahi hai jahan risk team sunna band kar deti hai.

**Q35. Diagnosis mein pehle prompt kyun dekhte hain?**
Kyunke prompt dobara parhna seconds ka kaam hai aur sab se aam wajah (under-specification) ko resolve karta hai. Task ko ghalat kehna aakhri step hai kyunke wo koshish ko khatam kar deta hai.

# Section D: Farq wale sawal

**Q36. Under-specification aur context overload mein farq?**
Under-specification **pehle jawab se** ghalat hota hai (prompt mein cheez thi hi nahi), fix hai kami add karna. Context overload mein shuru theek hota hai aur **session lamba hone par** kharab hota hai (purani instructions kamzor), fix hai restart ya summary. Behtar prompt overload mein kaam nahi karta.

**Q37. Stale configuration aur unstaffed gate mein kya mushtarak hai?**
Dono mein ek control sahi set hota hai, phir chupke se decay hota hai aur koi signal nahi aata. Isliye dono ka ilaaj ek hi hai: **scheduled read**. Source in dono ko ek hi ghalti ke do roop kehta hai (ye framing is book ki apni addition hai).

**Q38. Halo delegation aur over-delegation mein farq?**
Over-delegation bari chhatri hai: step ke risk se zyada AI ko dena. Halo delegation us ka ek roop hai: ye wajah ke pichla step achha gaya. Misaal: "summaries sahi thi to severity classification bhi AI karega". Summary aur classification alag steps hain.

**Q39. Skill, standing instruction aur knowledge base mein farq?**
**Skill** procedure hai (steps ka order, account level par, har Project mein chalti hai). **Standing instruction** rule hai (Project mein har run par lagta hai). **Knowledge base** reference files hain (jo Project parh sakta hai). Ek line ki instruction mein procedure daalne se order kho jata hai.

**Q40. Reversibility aur stakes mein farq?**
Reversibility poochta hai ke ghalti **undo** ho sakti hai ya nahi. Stakes poochta hai ke **bure case mein** ghalti ki cost kya hai. Ek step undo ho sakta hai magar phir bhi mehnga ho sakta hai, aur ek step sasta ho sakta hai magar undo nahi hota.

**Q41. AI-appropriate aur collaborative mein farq?**
AI-appropriate mein AI own karta hai aur nateeja agle step mein koi judge karta hai. Collaborative mein AI sirf **produce** karta hai aur ek **naam wala insaan** us step ko judge karta hai. Same step ek workflow mein AI-appropriate aur doosre mein collaborative ho sakta hai, agar uske baad koi khara hi na ho. (Misaal: contract mein playbook flags, vs expense mein travel policy check.)

**Q42. Consolidate aur promote mein farq?**
Consolidate **steps ki tadaad** kam karta hai (teen prompts ko ek mein milana). Promote **bache hue steps ki cost** kam karta hai (pattern ko configuration mein daalna). Pehle consolidate, kyunke jo step merge hone wala hai usay promote karna zaya mehnat hai.

**Q43. Synthesis aur calculation mein farq?**
Synthesis considerations jama kar ke options banana hai (AI isme acha hai). Calculation mein figure ki sahi hone ki tasdeeq page se nahi hoti, isliye wo compute hona chahiye.

**Q44. "Compute karna hai" aur "AI ko dena hai" mein farq?**
"Compute karna hai" **implementation** (kaun si cheez carry kare) ki baat hai. "AI ko dena hai" **ownership** (3 criteria) ki baat hai. In dono ko mix karne se high-stakes calculation bina review ke reh jati hai.

# Section E: Scenario sawal (sir aksar aise poochte hain)

**Q45. Ek team ne AI ko 4 mahine drafts likhte dekha, ab usay low-value responses seedha bhejne dena chahti hai. Kaun si ghalti?**
**Halo delegation.** Drafting ki quality draft ka evidence hai, bhejne ke faisle ka nahi. Aur bhejna undo nahi hota. (Ye unstaffed gate nahi, kyunke team khula faisla le rahi hai.)

**Q46. Fresh chat mein pehle hi jawab mein do payment terms ka zikr nahi. Wajah?**
**Under-specification.** Session fresh tha aur pehla jawab hi ghalat, to context overload aur stale configuration dono rule out (dono ko waqt chahiye).

**Q47. Manager har Friday refund queue ek batch mein bina cases khole approve karta hai, map "collaborative" kehta hai. Kya halat hai?**
Step **practically automated** hai. Collaborative step jiska koi real reviewer na ho automated step hai. Map wo likhta hai jo design kiya tha, jo chal raha hai wo nahi. Batching yahan optimisation nahi, control ka hata dena hai.

**Q48. Ek call checklist artifact 6 mahine baad 3 managers aur HR ke new-hire pack mein hai. Ye kya signal hai?**
**Escalation signal**: doosre log ab is par infrastructure ki tarah depend karte hain, to ye prompt-and-iterate se bahar hai aur developer ya architect ka kaam hai. (Model tier ya review gate is ka jawab nahi.)

**Q49. Teen coordinators ke weekly updates alag alag consistent hain, director har Monday ek ghanta unhein ek voice mein likhta hai. Kaun sa friction signal?**
**Variance.** Har ek ka apna output consistent hai, inconsistency sirf logon ke beech aur reviewer ke paas dikhti hai. Fix: shared Skill.

**Q50. Ek "report promptly deliver ho" requirement hai. Kya masla hai?**
Ye **ambiguous** hai. Do din aur do hafte dono kisi ke liye prompt hain, aur is ka check likha nahi ja sakta. Test: "kya main is ka check likh sakta hoon?" Nahi to wo abhi decide hi nahi hui.

**Q51. Koi shakhs "agle quarter ki exact sales figure" maangta hai aur AI ghalat batata hai. Kaun si cause?**
**Expectation mismatch**, magar sirf tab jab pehli 4 wajohat rule-out hon. Fix task badalna hai: range maango assumptions ke saath, ya adjustable model.

**Q52. Pichle quarter ke figures knowledge base mein hain aur is quarter ki report unhein quote karti hai. Kaun si cause aur kyun khatarnaak?**
**Stale configuration.** Khatarnaak isliye ke **silent** hai: koi error ya warning nahi aati, aur model ko pata hi nahi chalta ke jo diya wo purana hai.

**Q53. Dashboard ke totals ghalat nikle magar sahi lagte the. Kya masla aur fix?**
Totals **likhe gaye the, compute nahi hue.** Ye feature problem hai, behtar description se hal nahi hota. Fix: totals ko **code execution** mein daalna.

**Q54. Ek workflow ka severity classification AI ne kiya, phir usi severity ke mutabiq AI ne bina review ke response bhej diya. Kya galat hai?**
Do cheezein: severity classification **halo delegation** hai (summary acha tha, classification alag step), aur bhejna **over-delegation** hai ("low severity only" control nahi, kyunke severity usi system ne set ki jo ab bina review ke bhej raha hai, aur bhejna undo nahi hota).

# Section F: Rapid-fire (ek line mein jawab)

- **Design?** Tool se pehle requirements aur numbers tay karna.
- **Map?** Har step ka owner aur wajah.
- **Build?** Ideate, prototype, feedback, refine loop.
- **Diagnose?** Symptom kab aaya, us se wajah.
- **Persist?** Fix ko chat se nikal kar configuration mein daalna.
- **Communicate?** Kya karta hai batao, aur human gate ka naam lo.
- **Promotion?** Fix ko configuration mein le jana.
- **Window test?** Kya step ki saari zaroorat model ke samne rakh sakte ho?
- **Judgment step?** Jis ka input aap supply nahi kar sakte.
- **Over-delegation?** Step ke risk se zyada AI ko dena.
- **Unstaffed gate?** Review naam ki reh gayi.
- **Map owner?** Ek naam wala banda jo map ke sach hone ka jawab-deh hai.
- **Scheduled read?** Tay tareekh par map ka review.
- **Baseline?** Badalne se pehle ki naap.
- **Parallel run?** Purana aur naya saath chalana.
- **Friction?** Chhota repeated cost jo dekhna chhor diya.
- **Escalation signal?** Doosre log depend karne lagen.
- **Tier?** Model ka version, fast/cheap se slow/capable tak.
- **Sab se bara usool?** The output is not the verdict.

**Tip:** Agar sir kisi stage ya concept ko poochein aur aap atak jayein, to is order mein bolein: **(1) kya hai, (2) kyun zaroori hai, (3) kitni types ya steps hain aur naam, (4) ek misaal.** Isse jawab khud complete lagta hai.

A




