

# Section A: "X kya hai?"

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
