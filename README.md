
# AI Fluency: 

Source: *AI Fluency: A Crash Course* (Panaversity Agent Factory, agentfactory.panaversity.org/docs/ai-fluency-crash-course), jo Prof. Rick Dakan aur Prof. Joseph Feller ke AI Fluency Framework (Anthropic ke saath) par based hai. Is guide ke rules, definitions aur 4Ds course se hain. Chai, Sara aur Ahmed wali misalen, aur "agar ye na ho to kya hoga" wali wazahatein meri teaching hain, course ke lafz nahi. Jahan meri apni samajh hai, wahan likh diya hai.

## 1. Maqsad: hum AI Fluency kyun parh rahe hain

### Ek nayi colleague ki kahani (course se)

Aap ki team mein ek talented nayi colleague aati hai. Aap kehte hain: "AI agents par ek course outline bana do." Wo polished outline deti hai, magar PhD researchers ke liye, poore semester ka, aur hands-on practice ke bina. Wo incapable nahi thi. Aap ne audience, time, teaching style aur end goal bataya hi nahi tha.

AI ke saath yehi hota hai, ek farq ke saath: **insaan colleague ko ek baar bata do to agle mahine bhi yaad rehta hai. AI ek chat se doosri chat mein kuch yaad nahi rakhta.** Har nayi chat mein wo ek aisi colleague hai jo aap se kabhi mili hi nahi. Jo aap insaan ko ek baar batate, wo AI ko har baar batana hai, ya aisi jagah rakhna hai jahan AI khud parhe. Memory feature sirf notes save karke agli chat mein bhejta hai, model khud khali shuru karta hai.

### Do emails ka experiment (course se)

Pehle likho: "Write a welcome email for new members." Jawab theek hoga magar bilkul general. Phir likho: Karachi ke ek chhote women's cycling club ke naye members, nervous beginners, warm aur thoda funny, 150 words se kam, exclamation marks nahi, end mein Saturday 6am ki slow ride ka zikr. **Same model, same task, machine ke liye same 3 seconds.** Doosri email behtar hai.

Is se do sabaq milte hain:

1. Do results ke beech ka farq **aap se aaya, model se nahi.** Ye Description hai.
2. Aap doosri email ko behtar tabhi pehchan paye jab aap ko cycling clubs, nervous beginners ya Karachi ke baare mein kuch pata tha. Ye Discernment hai.

### AI Fluency ki taareef

AI fluency yani AI ke saath aise kaam karna jo ho:

- **Effective:** aap goal tak pahunchein.
- **Efficient:** waqt, mehnat aur tokens zaya na hon. (Tokens: wo chhote text ke tukray jo AI parhta aur likhta hai, aur jin ke hisaab se paisa lagta hai.)
- **Ethical:** fair aur honest istemal.
- **Safe:** logon, privacy, security aur zaroori information ki hifazat.

Is ka matlab **AI ke saath tez kaam karna nahi**, aur na model train karna, na magic prompts ka collection. Buniyad hai **achhe insani faisle**, AI ke aas paas.

Asaan likhein to 4Ds ek ek lafz mein: **Delegation = decide, Description = explain, Discernment = check, Diligence = own.**

### Engineers ke liye iska faida (course se)

- Agar aap ek AI assistant ke saath achha kaam nahi kar sakte, to aap wo system design karne ke liye tayyar nahi jo hazaron users ke liye action le. Chat mein practice, agent banane ki rehearsal hai.
- Chat ke 4Ds, Agent Factory mein engineering ban jate hain (section 11 mein table).
- Course ka jumla: techniques models ke saath badal jati hain, **chaaron competencies tikay rehne ke liye bani hain.**

### Agar ye skill na ho to kya hoga (meri wazahat)

Polished magar ghalat jawab accept ho jata hai, aap ka data ghalat jagah chala jata hai, aur wo kaam AI ko mil jata hai jo insaan ka tha. Ye sab course ke chaar beginner mistakes mein dikhte hain (section 9).

### Ek ehtiyat (course se)

Poora complete brief dene ke baad bhi jawab ke sahi hone ki zamanat nahi. AI fact ya source invent kar sakta hai aur phir bhi confident lagta hai. Behtar instructions aap ki odds barhate hain, output ko sach nahi banate. Isliye checking ek alag skill hai (Discernment).

## 2. AI ke saath kaam karne ke 3 tareeqe (modes)

Maqsad: ye samajhna ke kaam mein AI ko kitni azaadi di ja rahi hai. Farq is mein hai ke AI agla kya karna hai, ye khud kitna tay karta hai.

- **Automation:** AI wo task karta hai jo aap batate hain. Misal: "Is report ke 5 bullets bana do." Aap script writer ki tarah hain.
- **Augmentation:** aap aur AI mil kar sochte hain. Misal: business idea par brainstorming. AI thinking partner hai, aap co-creator.
- **Agency:** aap goal aur boundaries dete hain, AI bahut se steps khud tay karta hai. Misal: "Meri inbox sambhalo, routine messages ka jawab do, zaroori wale flag karo, aur jahan pakka na ho wahan mujh se poochho." Aap director hain, magar aksar aap har take dekh nahi rahe hote.

Course ke mutabiq agency ka matlab hai ke ek insaan AI ko is tarah configure kare ke wo **aane wale kaam (future)** khud kare, aksar **doosron ke liye (for others).** Isiliye agency mushkil hai: aap har faisla supervise nahi kar sakte, to judgment pehle se andar banani parti hai.

Koi mode khud-ba-khud behtar nahi. Ek project mein teeno ho sakte hain.

## 3. D1: Delegation (kaun sa kaam kis ka)

**Maqsad:** prompt likhne se pehle tay karna ke kaam kya hai aur insaan aur AI mein kaise bantega. Course ka jumla: **Delegation workflow design hai, sirf task offloading nahi.** Isliye ye pehla D hai.

Delegation ke 3 hisse hain (framework ki reference document pehle hisse ko "goal and task awareness" bhi kehti hai).

### 3.1 Problem awareness (kaam ko samjho)

AI se kuch maangne se pehle poochen: Goal kya hai? Kis ke liye hai? Success kaisa dikhta hai? Kya ghalat ho sakta hai? Kahan insani faisla zaroori hai?

Course ki misal: "Build me an invoice-chasing agent." AI kuch bana dega, magar asal sawal khule hain: kin customers ko contact karna hai? kitne din late par? kis tone mein? kitni raqam par insaan approve kare? dispute par kya hoga? agent sirf draft kare ya bhej bhi sakta hai? Ye **business sawal** hain, prompting ke sawal nahi.

**Agar ye na ho:** AI ko business policy khud guess karni parti hai.

### 3.2 Platform awareness (sahi tool chuno)

Har AI har kaam ke liye barabar nahi. Course ki misalen: mushkil multi-step masle ke liye **reasoning model**, current information ke liye **search-enabled assistant**, software kaam ke liye **coding agent** (project ki files parhta aur badalta hai), kai steps ke liye **agent-capable system**. Model ke naam yaad karne ki zaroorat nahi, market tezi se badalta hai. Aadat ye honi chahiye: "kya ye is kaam ka sahi tool hai?"

**Agar ye na ho:** aap ghalat tool se kaam lete hain (jaise current price ke liye aisa model jo search nahi karta).

### 3.3 Task delegation (kaam baanto)

Kaam ko hisson mein toro aur har hisse ka malik aur wajah tay karo. Course ki misal (course banana): audience aur goals tay karna **Human** (purpose aur judgment chahiye); structure suggest karna **AI + human** (AI breadth, human chunta); draft **AI**; facts verify karna **Human** (accountability author ki); lived experience **Human**; grammar **AI**; final approval **Human** (aap ka naam laga hai).

Sawal "kya AI ye kar sakta hai?" nahi. Sahi sawal: **kaun sa hissa AI kare, kaun sa main, aur kyun?**

**Agar ye na ho:** AI wo faisla kar leta hai jo insaan ka tha, aur aap ko pata bhi nahi chalta.

### Delegation ke teen "delegate" wale lafz (uljhan)

- **AI Fluency ka Delegation:** insani **faisla** ke kaun sa kaam kis ka.
- **Delegation Map** (Workflow Design course): wohi faisla, har step ke saath **likha hua** (AI, AI + human, ya human).
- **Delegation Loop** (Just Delegate It course): ek job AI ko dene ka 6 qadam wala rhythm.

### Ek wazahat: "kaun karega" aur "kaise karega"

"Pani ubalna AI kare, chakhna main" **Delegation** hai (kaun). "Pehle pani ubalo, phir patti" **Description ka Process** hai (kaise).

## 4. D2: Description (AI ko kya batana hai)

**Maqsad:** AI sirf wohi jaanta hai jo uske saamne hai. Jo aap ne nahi bataya, wo guess karta hai, aur ma'qool guess bhi ghalat ho sakti hai. Description sirf achha prompt likhna nahi, ye **context engineering** tak jata hai: AI ko jo bhi information chahiye (documents, examples, memory, policies, tools) us ka design.

Yaad: **What, How, How to work with me.**

### 4.1 Product description (kya chahiye)

Output ki qism, audience, format, length, tone, kin topics par focus, aur kya nahi chahiye. Course ki misal: "Summarize this report" ke bajaye "senior executives ke liye jin ke paas 10 minute hain, revenue trends, risks aur recommended actions par focus, chhote bullets, ek page, jo figure bohat badli use highlight, aur jargon nahi." Doosri request zyada smart nahi, **zyada mukammal** hai.

**Agar ye na ho:** result general aur bekaar (jaise pehli welcome email).

### 4.2 Process description (kaise karna hai)

Steps, order, method, misalen, aur khatam karne se pehle checks. Course ki misal: code review mein pehle correctness, phir security, aakhir mein style.

Course ka bara example: 3 vendors ke proposals. Sab ek request mein dene se AI extract, compare, score aur likhna ek hi pass mein kar deta hai, aur aap sirf aakhri result check kar sakte hain. Behtar: **ek request, ek step, har step ke baad check.** 1) sirf table banao (price, contract length, exit terms, support hours) aur ruko; 2) sirf us table se compare karo; 3) score do; 4) recommendation likho. **Jis step mein ghalti sab se zyada phailti hai (extraction) use pehle rakho**, kyunke ghalat price aage har cheez mein chala jata hai.

**Agar ye na ho:** ghalti beech mein chhup jati hai aur aakhir mein achhi dikhti hai.

### 4.3 Performance description (AI ka rawayya)

AI aap ke saath kaisa pesh aaye: mukhtasar ya tafseeli, challenge kare ya support, pehle sawal poochhe ya assumption le, uncertainty batayi jaye ya nahi. Course ki misal: "meri kamzor assumptions ko challenge karo, uncertainty flag karo, sirf politeness ke liye ittefaq mat karo." Is se AI "haan ji" machine se thinking partner ban jata hai.

Chat mein ye sirf aap ke liye hai. Agent mein wohi line **hazaron logon par** lagti hai (jaise tutor kabhi jawab pehle na de). Course ke lafz: chat mein bura Performance description dus minute ki jhunjhalahat hai, deployed agent mein wo **product** hai.

**Agar ye na ho:** AI polite agreement karta hai, ya baar baar wohi masla dohrata hai.

### "Check" Description mein bhi aur Discernment mein bhi?

- Description mein aap **AI ko hukm** dete hain ("pehle table banao aur ruko"). Ye kaam se **pehle** hai.
- Discernment mein aap **khud result jaanchte hain.** Ye kaam ke **baad** hai.

## 5. D3: Discernment (result chakhna)

**Maqsad:** AI ghalat jawab bhi usi pakke lehje mein deta hai. Ghalat jawab par warning label nahi hota. Discernment poochta hai: kya AI ne waqai kaam achha kiya? (Description poochta hai: kya maine kaam saaf samjhaya?)

**Automation bias** (course ka term): insaan ka rujhan ke jo jawab machine ne diya aur professional dikhta hai us par zyada bharosa kar lena. Course ke mutabiq fluent writing, link aur confident lehja saboot nahi.

### Ghalat jawab ke 4 nishan (course se)

1. **Bohat exact figure** jo aap ne diya hi nahi ("99.97% on-time"). Source kholo.
2. **Wahan confidence jahan expert hichkichata**, jaise "it depends" wale sawal par seedha haan. Poochen kya cheez jawab badal degi.
3. **Lambay output mein contradiction.** Shuru ko aakhir se milao.
4. **Aisi action jo hui hi nahi** ("maine email bhej di"). Jab tak tool bheji hui email, khola hua page ya test log na dikhaye, ye sirf ek jumla hai.

### 5.1 Product discernment (result achha hai?)

Chhe sawal: sahi hai? har important requirement follow hui? kuch missing? andar se mel khata? expert maanega? main apna naam laga sakta hoon? Aap ka domain knowledge yahan kaam aata hai (accountant ghalat assumption pakadta hai, programmer subtle bug). Result ke saath **dalil** bhi dekho: maangein assumptions, evidence aur decision criteria. Ye review ke liye pesh ki hui dalil hai, AI ki hidden thinking ka record nahi.

Jab jawab apni documents se aana ho, ye add karein: sirf attached documents se jawab do; agar likha nahi to "document mein nahi" kaho; har cheez ka heading aur jumla quote karo.

**Agar ye na ho:** polished ghalat jawab aage chala jata hai.

### 5.2 Process discernment (tareeqa kaam kar raha hai?)

Poori session dekho: kya AI meri feedback se seekh raha hai ya wohi ghalti dohra raha hai? kya main har turn wohi formatting theek kar raha hoon? kya main draft ko apne likhne se zyada edit kar raha hoon? Course ka saaf jawab: 20 minute steering jo ek ghanta bachaye faida hai; jo sirf 15 minute bachaye wo nuksan hai jo productive lagne ki wajah se faida samjha jata hai. Tareeqa kaam na kare to 3 qadam: Performance description badlo, tool badlo, ya kaam wapas le lo.

### 5.3 Performance discernment (AI akele kaam kare to?)

Sirf tab aata hai jab AI agency mein doosron ke liye kaam kare. Course ki misal: AI tutor har sawal ka sahi jawab deta hai, magar student jhijhakta hai to solution de deta hai aur koi seekhta nahi. Har jawab sahi, tutor bura. Ye ek chat mein nazar nahi aata, bohat saare cases ke pattern mein nazar aata hai, isliye ye infrastructure (evals) ban jata hai.

### Description aur Discernment ka loop

Aap batate hain, AI banata hai, aap parakhte hain, aap batate hain kya badalna hai, AI dobara karta hai. Pehla jawab draft hota hai, finish line nahi. Feedback ka pattern: **Problem, Why it matters, Direction.** Kamzor: "ghalat hai, dobara karo." Behtar: "doosra section enterprise customers maan kar chal raha hai (problem). Hamara audience solo founders hai, salah mehngi hai (why). Is section ko ek insaan ke tang budget wale business ke liye likho (direction)."

Course ki ek khoobsurat misal: ek finding (tickets double, team nahi barhi, first reply 4 ghante se 9 ghante) ko board ke liye likhwao (number, wajah, faisla) aur support team ke liye (kya badla, aap ki ghalti nahi, Monday ko kya karna hai). Draft aksar isliye theek nahi hota ke ghalat reader ke liye likha gaya.

### Ghalti kis ki? (aap ka sawal)

- **Meri instruction ghalat thi** (maine 2 cup likha, chahiye 1 thi): Description theek karo. AI ne wohi kiya jo kaha gaya.
- **AI ki ek khaas ghalti:** AI ko batao aur theek karwao (ye step meri teaching hai, course ke lafz nahi).
- **Wohi qism ki ghalti baar baar:** tool badlo, yani Delegation ke Platform awareness par wapas.
- **Sab kuch try kiya, phir bhi nahi:** kaam wapas le lo. Course ke mutabiq ye bhi fluency hai, naakami nahi.
- **Na meri na AI ki:** Delegation hi ghalat thi (ghalat tool, ya AI ko wo hissa dena hi nahi chahiye tha). Course khud kehta hai ke Discernment kabhi Delegation ki ghalti dikha deta hai.

### Review ke 3 anjaam

Har review in mein se ek par khatam hoti hai: **ready to use, needs revision, needs human override.** Agla message likhne se pehle faisla kar lo, is se "ek aur chhota change" ka loop band hota hai.

## 6. D4: Diligence (zimmedari)

**Maqsad:** pehle teen Ds behtar result ke liye hain. Diligence alag sawal poochta hai: **kya mujhe AI is tarah istemal karna bhi chahiye, aur result ki zimmedari kaun uthayega?** Ye AI ke baare mein nahi, **aap ke baare mein** hai.

Course ki misal: ek lecturer AI se term-end feedback likhwata hai. Likhai bohat achhi hai. Magar usne students ke naam, grades aur disciplinary notes ek aisi consumer AI service mein paste kiye jo university ne approve nahi ki thi, aur students ko ye nahi bataya ke AI ne comments likhe. Output achha ho sakta hai, AI ka istemal phir bhi ghalat hai.

### 6.1 Creation diligence (kaam se pehle aur dauran)

AI ko kuch dene se pehle: is mein personal data hai? confidential information? mujhe ye is tool mein daalne ki ijazat hai? tool meri organization ne approve kiya? koi legal ya contractual pabandi?

**Redaction** (course ka term): pehchan karwane wali details hatana, aur wo pattern rakhna jo kaam ko chahiye. AI ko pattern chahiye, shakhs nahi. Ye do taraf se fail hoti hai: bohat zyada hata diya to kaam nahi ho sakta; bohat kam hataya to details ka mel phir bhi ek shakhs tak pahunchata hai ("wo akeli student jo week 3 ki lab miss kar gayi"). Test: sirf paste kiya hua text parh kar koi andaza laga sakta hai ke ye kis ke baare mein hai? Data saaf karne se tool ka sawal hal nahi hota.

**Agar ye na ho:** data unapproved jagah chala jata hai, aur baad mein wapas nahi aata.

### 6.2 Transparency diligence (AI ka role sach batana)

Har AI-assisted kaam ka elaan zaroori nahi. Magar jab AI **doosre logon ko mutassir** kare (academic kaam, hiring, customer communications, medical ya financial advice, professional reports) to disclosure ka sawal uthta hai. Rules context, law aur professional standard par depend karte hain. Course ka usool: **jitna zyada AI-assisted result doosron ko mutassir kare, utni zyada transparency ki zaroorat.** Transparency ka matlab poora workflow publish karna nahi, matlab hai logon ko AI ke role ke baare mein **gumrah na karna**, jab wo role matter karta ho.

Ye "data mein kisi ka naam to nahi" wala sawal nahi. Wo privacy hai (Creation aur Deployment mein aati hai). Transparency ka sawal hai: **kya logon ko batana chahiye ke AI ne madad ki?**

### 6.3 Deployment diligence (bhejne se pehle check)

Publish, send, execute ya kisi faisle mein istemal se pehle check karo. Jitne zyada log result tak pahunchen, utni zyada checking, aur jo qadam wapas nahi ho sakta (payment bhejna, folder delete karna) uska check **karne se pehle** hota hai, kyunke baad mein koi reviewer nahi. Facts, sources, calculations, bias, permissions, policy, aur bade asar wale actions ke liye insani approval.

**The numbers rule (course se):** jis number par faisla ho (total, percentage) wo **compute hona chahiye, generate nahi.** AI column ko spreadsheet ki tarah jama nahi karta, wo ma'qool dikhne wala total predict karta hai, to total ghalat ho sakta hai jabke har line sahi ho. Number spreadsheet, calculator ya wo code se lo jo AI ne chalaya aur dikhaya, phir inputs check karo.

**Final test:** "Kya main isay confidently apna naam laga kar de sakta hoon?" Agar jawab "pata nahi" ho (case saaf nahi), to 4 sawal: kaun mutassir hota hai (un sameet jo result kabhi nahi dekhenge)? un ke saath kya ghalat ho sakta hai aur kya wo pehchan paayenge? fair nateeja kaisa hoga? kya aur kis ko disclose karna hai? Agar jawab de sakte ho to faisla karo aur likho, warna us ko escalate karo jis ke paas ye faisla hai. Andaza lagana wahi ek raasta hai jo ek ghair-wazeh case ko aap ki ghalti bana deta hai.

**Course ka sab se ahem jumla: AI kaam automate kar sakta hai, accountability automate nahi kar sakta.** Agar coding assistant security flaw daale aur engineer ship kar de, to engineer aur organization zimmedar hain.

**Agar ye na ho:** result achha ho tab bhi privacy tooti, logon ko pata nahi chala, ya ghalat result bhej diya, aur jawab aap ko dena parta hai.

## 7. Poora raasta (steps ka order)

Course Diligence ko "aakhir ka checkbox" nahi, balki poore workflow ke aas paas batata hai. Ye 6 qadam wali tarteeb meri teaching ka tareeqa hai, taake Diligence ke teen waqt saaf nazar aayein:

1. **Delegation:** goal, tool aur kaam ki taqseem tay karo. (AI ko abhi kuch nahi diya.)
2. **Creation diligence:** AI ko data dene se pehle tool aur privacy check, redaction.
3. **Description:** product, process aur performance batao.
4. **AI kaam karta hai.**
5. **Discernment:** result chakho, ghalti pakro.
6. **Deployment diligence** (aur jahan zaroori ho Transparency): bhejne se pehle check, numbers compute, naam laga sakta hoon?

Ye seedhi line nahi, **loop** hai. Masla jis step ka ho wahin wapas jao: instruction ghalat to Description; tool ghalat to Delegation (Platform); kaam hi AI ka nahi tha to Delegation (Task); data ghalat jagah gaya to Creation se pehle rokna tha (baad mein theek nahi hota).

## 8. Poora example: Sara teacher (meri kahani)

Sara ko term ke end par 30 students ke parents ke liye feedback likhni hai.

**1. Delegation.** Goal: har parent ko 4-5 jumlon ki saaf, mehrbaan feedback mile. Kya ghalat ho sakta hai: AI koi aisi baat likh de jo bachhe ne kabhi ki hi nahi. Insani faisla: disciplinary baatein aur final feedback Sara ki. Tool: aam writing assistant kaafi. Pehla draft AI, facts check aur bhejna Sara. *Agar ghalti:* sab AI par chhor diya to AI mizaj ke baare mein faisle likh deta; wapas Delegation Task par.

**2. Creation.** Data paste karne se pehle: kya school ne ye tool approve kiya? Phir redaction: naam hata kar "ek student jis ke numbers 60 se 70 ke beech hain aur jo sawal poochne se jhijhakta hai." "Akeli bachi jo sports day mein nahi aayi" jaise detail se bachna. *Agar ghalti:* naam, marks aur disciplinary notes unapproved app mein chale gaye; baad mein theek nahi hota.

**3. Description.** Product: parents ke liye 4-5 jumle, pehle ek achhi baat, phir ek mehnat wali cheez. Process: pehle sirf ek student ki feedback likho aur ruko. Performance: jo maine nahi batayi wo mat likho, aur shak ho to poochho. *Agar ghalti:* audience na batao to general feedback; 30 ek saath maangi to ek ghalat template sab mein.

**4. AI kaam karta hai.**

**5. Discernment.** AI ne likha "Ahmed ne science fair mein hissa liya." Ye ek bohat khaas baat thi jo Sara ne di hi nahi. Feedback: science fair ka zikr galat hai (problem), parents us par bharosa karenge (why), sirf wo likho jo maine batayi (direction). Phir poochna: ye meri ghalti thi (instruction mein "sirf wo likho" nahi tha) ya AI ki? *Agar chakhti hi nahi:* ghalat baat parents tak jati.

**6. Deployment.** Har feedback bhejne se pehle khud parhna. Attendance percentage spreadsheet se compute karna. School ki policy dekhna ke parents ko AI ke role ke baare mein batana hai ya nahi. Aakhri sawal: kya main isay apna naam laga kar de sakti hoon?

## 9. Chaar aam beginner ghaltiyan (course se)

1. **Problem define kiye bina prompt likhna:** Delegation chhoota. Fix: goal, audience, constraints aur human aur AI ka split pehle.
2. **Pehle jawab ko final maan lena:** Description aur Discernment ka loop chhoota. Fix: result dekho, specific feedback do, dobara chalao.
3. **Polished jawab ko sahi maan lena:** Discernment chhoota. Fix: important facts, assumptions, calculations aur sources verify karo.
4. **Privacy ya accountability baad mein sochna:** Diligence chhoota. Fix: data, disclosure, approval aur accountability ke rules deploy karne se pehle tay karo.

## 10. Roz ka beginner checklist (course se)

- **Delegate:** goal kya hai? AI kya kare? mere paas kya rahe?
- **Describe:** AI ko kaunsa output, context, method aur behavior chahiye?
- **Discern:** mujhe kaise pata chalega ke jawab sahi, mukammal aur kaam ka hai?
- **Be diligent:** data safe hai? AI ke role ka disclosure chahiye? kaun approve karega aur result ka malik kaun hai?

Course ke mutabiq ye har chhote kaam ke liye paperwork nahi, maqsad ye hai ke chaaron sawal automatic ho jayein.

## 11. Chat se Engineering tak (course se)

- **Delegation:** chat mein "AI se kya karwana hai"; engineering mein Digital FTE ka scope aur human-AI boundary. Problem awareness specification ban jata hai (goal, constraints, risks, definition of done).
- **Description:** chat mein instructions aur context; engineering mein system prompts, skills (SKILL.md), context engineering aur System of Record.
- **Discernment:** chat mein jawab ka review; engineering mein evals, monitoring, sampling aur release gates.
- **Diligence:** chat mein data ki hifazat aur result ki zimmedari; engineering mein governance, permissions, audit logs, disclosure aur human review.

Digital FTE: ek AI worker jo doosre logon ke liye ek tay-shuda job karta hai (FTE: full-time equivalent).

Course ka ek aur ahem nuqta: koi policy tabhi chalti hai jab approved tool utna hi aasani se mile jitna wo tool jo log pehle se khol kar baithe hain. Lecturer ki consumer service ek click door thi. Agar approved tool ke liye form aur ek hafta chahiye, to aasan raasta policy ki kamzori hai, sirf kisi ki ghalti nahi.

## 12. 10-80-10 (book ka extension)

10-80-10 AI Fluency Framework ka hissa nahi, ye is book ka apna rule hai, jis se course 4Ds ko jorta hai. **Pehle 10%** direction tay karo (Delegation, Description), **beech ka 80%** AI se kaam karwao aur steer karo (Description, Discernment), **aakhri 10%** result judge karo (Discernment), aur **poore 100% par** Diligence. Chaaron Ds ka ek loop banana bhi book ka extension hai; original authors Description aur Discernment ka loop sikhate hain.

## 13. Aam uljhanein, saaf

- **AI Fluency tez kaam karna nahi.** Effective, efficient, ethical, safe.
- **Fluency, Delegation Map aur Delegation Loop alag cheezein hain.** Fluency 4 salahiyatein; Map faisle ka likha hua roop (Workflow Design); Loop ek job chalane ka rhythm (Just Delegate It).
- **Delegation = kaun karega. Description Process = kaise karega.**
- **"Check" Description mein AI ko hukm hai; Discernment mein aap ka khud ka kaam.**
- **Performance "AI mujh se poochhe" tak mehdood nahi.** Ye AI ke poore rawaiye ki baat hai (challenge, uncertainty, ittefaq ya na).
- **Diligence AI ka kaam nahi, aap ka.** Aur ye teen waqt mein hai: kaam se pehle (Creation), logon ke liye (Transparency), bhejne se pehle (Deployment).
- **Creation ka matlab project banana nahi**, AI ko kuch dene se pehle ke checks. Delegation phir bhi pehla qadam hai.
- **Transparency privacy nahi.** Transparency = AI ke role ke baare mein sach batana.

## 14. Quick self-check (course ke 10 sawal, jawab ke saath)

1. **AI fluency ki 4 qualities?** Effective, efficient, ethical, safe.
2. **Automation, augmentation aur agency mein farq?** Automation defined task chalata hai; augmentation aap ke saath thinking partner hai; agency goal ki taraf zyada azaadi se steps khud chunti hai.
3. **Delegation ke 3 hisse?** Problem awareness, platform awareness, task delegation.
4. **Description ke 3 hisse?** Product, process, performance description.
5. **Confident jawab ko bhi verify kyun?** Sounding right is not the same as being correct. Fluent wording facts, assumptions ya reasoning verify nahi karti.
6. **Discernment ke 3 hisse?** Product, process, performance discernment.
7. **Diligence ke 3 hisse?** Creation, transparency, deployment diligence.
8. **Shipping se pehle ka sawal?** "Would I confidently put my name on this?"
9. **4D loop ek jumle mein?** Decide what AI should do, describe the work, evaluate what comes back, aur poore process ki zimmedari lo.
10. **Discernment engineering mein kaise ban jata hai?** Evals, monitoring, sampling aur review gates.

**Poore course ka ek jumla:** Decide what AI should do. Describe the work clearly. Check what comes back. Own what happens next.

## 15. References

- AI Fluency: A Crash Course (Panaversity Agent Factory): https://agentfactory.panaversity.org/docs/ai-fluency-crash-course
- The AI Fluency Framework (authors ki site): https://aifluencyframework.org/
- AI Fluency: Framework and Foundations (free, Claude Academy): https://academy.claude.com/courses/ai-fluency-framework-foundations
- Framework for AI Fluency: Practical Overview Document: https://ringling.libguides.com/ai/framework

Framework ke authors: Prof. Rick Dakan aur Prof. Joseph Feller. Course ke mutabiq unka original course Anthropic ke saath banaya gaya aur CC BY-NC-SA 4.0 ke tahat release hai. Agent Factory ke mappings, chat-to-factory scaling aur 4D loop ki framing book ke extensions hain.
