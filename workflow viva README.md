

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

**Isko kaise yaad rakhein:** 23 problems aur 23 solutions hain. Agar viva mein koi concept poocha jaye, to pehle ye batayein ke **wo kis problem ke liye bana**, phir uska solution. Isse definition khud yaad aa jati hai.

Agar aap chahein to agla step ye ho sakta hai: har solution (S1 se S23) par viva ke **sawal aur jawab**, isi problem-solution style mein.
