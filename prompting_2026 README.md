Aapki paste ki hui file mein poora lesson tha, is liye ab Concepts 10–13 bhi parh liye hain. **Ab koi concept missing nahi.** Neeche poora lesson aik kahani ki tarah hai: har concept agle ki wajah banta hai.

## Kahani ki shuruaat: Hum yeh kyun parh rahe hain?

Zyada tar log AI ko Google ki tarah use karte hain: chhota sawal, jaldi jawab, aage. Trivia ke liye yeh chal jata hai, lekin asal kaam mein fail ho jata hai. Power users aur aam users mein farq dimaagh ka nahi, **chand aadaton** ka hai. Yeh lesson wahi 13 aadatein sikhata hai, 4 parts mein.

**Poori kahani ki buniyaad aik fact hai: Model stateless hai.** Woh turns ke darmiyan apna kuch yaad nahi rakhta, aur har dafa sirf usi text se jawab deta hai jo us waqt uske saamne hai. Is liye har "advanced technique" asal mein do mein se aik kaam hai: **sahi context andar daalo, ghalat context bahar rakho.**

**2022 se ab tak 8 cheezein badli hain:**
- Context window lagbhag 1000 guna bari ho gayi.
- Reasoning mode aa gaya.
- Web search built-in tool ban gaya.
- Code execution bhi built-in tool ban gaya.
- Images, files aur audio ab normal input hain.
- Tools ab aapke baare mein memory rakhte hain.
- Desktop apps aa gayi hain.
- Developers ke liye command-line agents aa gaye hain.

## Part 1: AI ko pata kaise hota hai?

**Concept 1: Novice vs Power user.** Kahani yahan se shuru hoti hai: aik hi sawal, lekin briefing alag ho to jawab alag aata hai.
- AI pehle din ka smart colleague hai jo aapke baare mein kuch nahi jaanta. Har nayi chat mein woh zero se shuru karta hai, aur baat samajh na aaye to poochhne ke bajaye guess karta hai.
- **Briefing ke 4 hisse:** Files, goal, limits, exact ask. Novice sirf aakhri hissa deta hai.
- **Sycophancy:** AI ki aadat ke woh wahi kahe jo aap sunna chahte hain.
- **Rubric:** Check karne ke points ki list, har point ka alag score. Rubric ke saath tie-dye business idea ko 100 mein se sirf 8 mile.
- **Slop:** Upar se smooth lekin andar se khaali text.

**Concept 2: Pretrained knowledge.** Ab sawal uthta hai: Jab AI jawab deta hai, woh aata kahan se hai? Pehla source uski training hai.
- **Pretrained knowledge:** Training text se jawab, kuch search kiye baghair.
- AI ne duniya mein reh kar nahi, text parh kar seekha. Jis topic par internet par zyada likha gaya, us par jawab zyada reliable hai.
  - **Strong:** Cooking, movies.
  - **Sparse:** Quasars, Cantonese, regional history.
  - **Absent:** Company ka private data, cutoff ke baad ki baatein.
- **Knowledge cutoff:** Woh date jahan training text khatam hoti hai.
- Typos se jawab nahi bigarta. Lekin internet ki ghalat baatein (**absorbed errors**) bhi AI ne seekh li hain, is liye important baat primary source se check karein.
- **Confidence is not correctness.** Nani ke gaon wale khel ke rules AI ne doosre ilaqon ke khelon ko mila kar bana diye.

**Concept 3: 3 retrieval modes.** Agar training mein jawab nahi, to AI bahar se dhoondta hai. Jawab aane ke teen raaste hain:
- **Pretrained:** Sirf training se.
- **Web search:** Kuch live pages parhta hai. Purana source bhi utha sakta hai, aur aksar poore page ke bajaye kisi chhote model ki banayi summary parhta hai.
- **Deep research:** Kai minute tak darjanon sources parh kar report banata hai.
- Aapki wording mode chunti hai: "What is" se pretrained, "latest" se web search, "research thoroughly" se deep research.
- **Do fixes:** Source types khud batayein, aur har claim ke saath exact quote maangein.
- **Google ya AI:** Link chahiye to Google, kai sources ka mila hua answer chahiye to AI.

## Part 2: AI se achhi tarah baat karna

**Concept 4: Context is the whole game.** Ab pata chal gaya ke AI sirf saamne rakha text dekhta hai. To agla sawal yeh hai: saamne kya rakha jaye?
- **Context window:** Woh sab jo model aik jawab likhte waqt dekh sakta hai. Is ka size **tokens** mein ginte hain; token aik word se thoda chhota text ka tukda hai.
- **6 layers:**
  - **System prompt:** Company ki chhupi hui instructions. Waiter ki briefing ki tarah.
  - **Tool descriptions.**
  - **Aapka prompt.**
  - **Chat history.**
  - **Files.**
  - **Memory:** Tool ka aapke baare mein likha hua note. Model ab bhi stateless hai.
- **Custom instructions:** Chhoti rakhein aur waqtan fawaqtan prune karein.
- **Context checklist:** Document, constraint, pichhla context, format, audience. Faltu files bhi nikalein.
- **Context rot:** Aik lambi chat mein bahut se topics hon to quality gir jati hai. **Compacting:** Purani baaton ki jagah summary aa jati hai. Hal: rescue ke bajaye nayi chat.
- **Projects:** Files aur instructions aik dafa set karein; har chat unhein le leti hai. Confidential data memory mein na jaane dein.

**Concept 5: Reasoning ("think hard").** Context de diya. Lekin mushkil sawal par AI ko sochne ka waqt bhi chahiye.
- **Reasoning:** Final answer se pehle model ki apni working.
- **Extended thinking:** Zyada der sochna; model kai approaches try kar ke apna kaam check karta hai.
- On karne ke 3 tareeqe: "think hard" likhein, thinking switch dabayein, ya tool khud on kar de.
- Chhote kaamon ke liye nahi: yeh slow hai aur zyada usage budget kharch karta hai.
- AI jitna lamba task kar sakta hai, woh lagbhag har 7 mahine mein double ho raha hai.

**Concept 6: Sycophancy.** AI soch kar jawab de bhi de, to woh aapko khush karne ki taraf jhukta hai.
- **Wajah:** Thumbs-up feedback par training.
- **Biased words:** Find, defend, confirm, prove. **Neutral words:** Evaluate, compare, critique, list both sides.
- AI ko "I don't know" kehne ki ijazat dein.
- **Rubric + force a number:** Har criterion ka 1–10 score. "There is always a next level."

**Concept 7: Brainstorm-iterate loop.** Achha aur sacha jawab mil gaya. Lekin pehla jawab average hota hai; behtar kaise banayein?
- **Loop:** Context → 3–5 options → feedback → naye options → aik option poora develop karein.
- **Outline before drafting:** Asal taqat outline par hoti hai. Score lagbhag 9.5 par ruk jaye to stop.
- **Diagnosis:** Batayein kaunsa hissa fail hua, sirf woh badlein.
- **Pehle ilaqa map karein:** Competitors, pichhli research, mojooda tareeqe.
- **4 kinds of ask:** Brainstorming mein format loose rakhein, drafting mein sab tight. Research aur analysis mein apna expected jawab kabhi na batayein.

## Part 3: Text se aage

**Concept 8: Multimodal.** Ab AI sirf text nahi; images, audio aur files bhi.
- **Image input:** Overall scene mein acha, bareek detail aur ginti mein kamzor. Totals hamesha check karein.
- **Diffusion model:** Noise se shuru kar ke step by step image banata hai.
- **Visual vocabulary:** Cinematic, watercolor jaise words controls hain. Ghalat text, chhe ungliyan aur aspect ratio par nazar rakhein.
- **[unclear] technique:** Jo samajh na aaye, AI usay mark kare, guess na kare.
- **SVG diagram workflow:** Claude se structure, ChatGPT ya Gemini se design.
- **Audio:** Meeting recording se decisions aur action items nikalwayein. Doctor ke SOAP note mein AI ne typing hatayi, judgment doctor ka raha.

**Concept 9: Aik prompt se app.** AI dekh aur sun sakta hai, aur ab bana bhi sakta hai.
- **Artifact:** Chat se bani chalti cheez jo edit, share aur download ho sakti hai. Claude mein Artifacts, ChatGPT aur Gemini mein Canvas.
- **Recipe:** Goal, Input, Output.
- Aik screen ki app jis mein accounts ya bahar ki services na hon, ban jati hai. Online multiplayer ke liye real engineering chahiye.

**Concept 10: Data analysis.** AI code likh kar app banata hai, to code chala kar hisaab bhi kar sakta hai.
- **Code execution:** Model program likh kar chalata hai. Calculator precise hai; model sirf chunta hai ke kya calculate karna hai.
- **Silent failure:** Chhote sawal par code skip kar ke andaza laga deta hai.
- **3 habits:**
  - "Write and run code. Show me the code you ran."
  - Check karein ke code block mojood hai.
  - Pehle row count, column names aur date range maangein.
- **CSV:** Rows aur columns wali saadi spreadsheet file.
- **Code chalne ke baad bhi check karein:** Totals (ghalat column jud gaya ho), graph ke labels, aur ghalat samjha hua column (jaise TXN_AMT). AI ko sharp junior analyst samjhein.

## Part 4: Safe kaam aur sahi tool

**Concept 11: AI desktop apps.** Ab AI chat se nikal kar aapke computer ki files tak pohanch gaya hai, to khatra bhi barh gaya.
- **AI desktop apps:** Cowork, OpenWork. Aapki ijazat se files dhoondti, parhti aur un par kaam karti hain.
- **4 steps:** Task batayein → action nahi, plan maangein → plan review aur edit karein → phir approve karein.
- **2 khatre:** Deleted files aksar recycle bin mein nahi jatin. Edited file ki history sirf tab bachti hai jab **version control** ho (software jo har purana version save karta hai).
- Sab se chhota folder dein; "full disk access" kabhi nahi.
- **Permission ladder:**
  - Pehle aik chhote folder ka sirf read access.
  - 2–3 kamyab runs ke baad aik folder mein write.
  - Aik saaf hafte ke baad project tree.
  - Aakhir mein specific permissions; "jo chahe karo" kabhi nahi.
- Scope track record ke hisaab se barhta hai, company par bharose se nahi.
- **Note:** Backup copy aur nayi file mein output wale rules Code You Never Write ke hain, is lesson ke nahi.

**Concept 12: Cost, speed aur model.** Ab sawal hai: kis kaam ke liye kaunsa tool, aur kitna kharcha?
- **Cost stack (sasta se mehnga):** Text (seconds, cent ka hissa) → speech → images → video (minutes, dollars tak). Video text se lagbhag 16 guna mehnga hai. Deep research kuch minute leta hai.
- Images aur video mein har round mehnga hai, is liye prompt pehle hi achha banayein.
- Free tier is page ke prompts ke liye kaafi hai.
- **Jagged:** Har model alag kaam mein aage hota hai, aur leader har kuch mahine mein badalta hai. Koi aik best model nahi.
- **Model ladder:** Aik company ke fast, medium aur heavy models. Chhote kaam par flagship ya mushkil kaam par sasta model, dono nuqsan dete hain.
- **Arena:** Public leaderboard jahan log do naam chhupe jawabon mein vote karte hain. Mahine mein aik dafa dekhein. Lekin yeh charm ko inaam deta hai, aur zaroori nahi ke voters ka kaam aapka kaam ho.
- **Weights:** Model ke andar trained numbers. DeepSeek ke weights public hain.
- **API:** Aik program ka doosre ko call karna. Meta AI ka public API abhi nahi hai.
- Meta AI aapke inputs training mein use kar sakta hai, is liye private data us mein na dein.
- **3 habits:** Do tabs khule rakhein, prompt notebook rakhein, aur jab model ghalat ho to note karein.
- **Aapke model list se link:** Grok aur Kimi bhi alag families hain, is liye cross-checking mein kaam aate hain.

**Concept 13: Models checking models.** Jab koi expert ya answer key na ho, to quality kaise jaanchein? Kahani yahan khatam hoti hai.
- **Model families:** Aik company ke saare models. Claude, ChatGPT, Gemini, Grok, Meta aur DeepSeek alag families hain.
- Do Claude models aapas mein check karein to cross-checking nahi, kyunki unki aadatein milti hain.
- **Aap pichhli dafa sahi the:** Lesson kehta hai alag families ke alag blind spots hote hain, kyunki unhein alag data par, alag ahdaaf wali teams ne train kiya.
- **A/B test:** Aik prompt 2–3 models mein bhej kar compare karna.
- **Recipe:**
  - Best model se poore context ke saath draft banwayein.
  - Usi se rubric par 1–10 grade karwayein aur apni suggestions lagwayein, jab tak score lagbhag 9 par na ruk jaye.
  - Doosri family ko wohi rubric dein.
  - Doosre ki critique pehle model ko dein; woh faisla kare kya lena hai.
  - High stakes ho to teesri family se bhi check karwayein.
  - Do alag models mein target score ho jaye to ruk jayein.
- **3 levels:** Rubric critique → aik model ka self-critique loop → multi-model loop. Jitna ghalti ka nuqsan zyada, utna bhaari level.
- **Privacy:** Har tool ki data policy check karein. **NDA** (raaz rakhne ka signed muahida) wala data sirf checked tools mein dalein.
- **Honest caveat:** Teen models bhi aik hi baat par ghalat ho sakte hain, kyunki unka training data aapki soch se zyada milta hai. **Score progress signal hai, truth signal nahi.** Legal, medical, financial ya kisi asal insaan ke baare mein claims insaani expert hi check kare.
- **Viva line:** "Models check each other for craft. Humans check the facts that matter."

## Kahani ka nateeja (yeh line yaad kar lein)

Poora lesson aik hi move ke 12 roop hain: **"Get the right context in, keep the wrong context out."**

**Yaad rakhne ki chain:** Briefing do (1) → jaano jawab kahan se aata hai (2, 3) → sahi context do (4) → sochne do (5) → khushamad hatao (6) → loop se behtar karo (7) → text se aage (8, 9, 10) → files mein ehtiyaat (11) → sahi tool chuno (12) → doosre model se check karo (13).

Aap chahein to agla step practice kar sakte hain: har concept par 2–3 viva sawal aur scenario MCQs.
