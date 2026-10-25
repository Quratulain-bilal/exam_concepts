

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
