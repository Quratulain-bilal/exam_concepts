

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

<img width="1600" height="2090" alt="download" src="https://github.com/user-attachments/assets/a7b7a845-315d-48ea-a689-f7e90ea2a689" />

<svg xmlns="http://www.w3.org/2000/svg" width="1600" height="2090" viewBox="0 0 1600 2090">
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

  <rect width="1600" height="2090" fill="#f6f7fb"/>

  <!-- Title -->
  <text x="800" y="72" class="title" text-anchor="middle">AI Prompting in 2026 — Big Picture</text>
  <text x="800" y="112" class="sub" text-anchor="middle">13 concepts · 4 parts · 1 kahani</text>

  <!-- Foundation -->
  <rect x="40" y="140" width="1520" height="122" rx="18" fill="#1d2433"/>
  <text x="70" y="182" class="w" font-size="18" letter-spacing="2" opacity="0.75">BUNIYAAD</text>
  <text x="70" y="222" class="w" font-size="28" font-weight="700">Model STATELESS hai</text>
  <text x="70" y="250" class="w" font-size="18" opacity="0.85">Apni koi memory nahi; sirf saamne wala text</text>
  <rect x="560" y="158" width="980" height="86" rx="14" fill="#374151" stroke="#9ca3af" stroke-dasharray="7 5"/>
  <text x="1050" y="196" class="w" font-size="27" font-weight="700" text-anchor="middle">“Get the right context in, keep the wrong context out.”</text>
  <text x="1050" y="228" class="w" font-size="19" text-anchor="middle" opacity="0.85">Sahi context andar daalo, ghalat bahar rakho. Poora lesson isi aik move ke roop hain.</text>

  <!-- Chain -->
  <text x="800" y="296" text-anchor="middle" font-size="20" font-weight="600" fill="#5b6475">Brief karo → Jawab kahan se? → Context do → Sochne do → Sach bulwao → Loop → Text se aage → Ehtiyaat → Sahi tool → Check</text>

  <!-- ================= PART 1 ================= -->
  <rect x="40" y="315" width="745" height="745" rx="18" fill="#eef4ff" stroke="#2563eb" stroke-width="3"/>
  <text x="62" y="360" class="h" fill="#2563eb">PART 1 · AI ko pata kaise hota hai?</text>

  <g transform="translate(55,385)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#2563eb"/>
    <circle cx="40" cy="36" r="18" fill="#2563eb"/><text x="40" y="43" class="n">1</text>
    <text x="68" y="44" class="t">Novice vs Power user</text>
    <text x="28" y="80" class="l">Prompt sawal nahi, BRIEFING hai: Files + Goal + Limits + Ask</text>
    <text x="28" y="107" class="l">Sycophancy (haan-mein-haan) · Rubric (score) · Slop (khaali)</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Pehle din ka smart colleague; samajh na aaye to guess karta hai</text>
  </g>

  <g transform="translate(55,552)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#2563eb"/>
    <circle cx="40" cy="36" r="18" fill="#2563eb"/><text x="40" y="43" class="n">2</text>
    <text x="68" y="44" class="t">Pretrained knowledge</text>
    <text x="28" y="80" class="l">AI ne jee kar nahi, PARH kar seekha (internet text)</text>
    <text x="28" y="107" class="l">Strong · Sparse · Absent  |  Knowledge cutoff = aakhri date</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Confidence ≠ Correctness. “Isay kaise pata hoga?”</text>
  </g>

  <g transform="translate(55,719)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#2563eb"/>
    <circle cx="40" cy="36" r="18" fill="#2563eb"/><text x="40" y="43" class="n">3</text>
    <text x="68" y="44" class="t">3 Retrieval modes</text>
    <text x="28" y="80" class="l">Pretrained → Web search → Deep research</text>
    <text x="28" y="107" class="l">Wording mode chunti hai · Source types + exact quotes maango</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Link chahiye = Google · Mila hua answer chahiye = AI</text>
  </g>

  <g transform="translate(55,886)">
    <rect width="715" height="155" rx="14" fill="#ffffff" stroke="#bfd3fb" stroke-dasharray="6 5"/>
    <text x="28" y="44" class="t" fill="#2563eb">Part 1 ka sabaq</text>
    <text x="28" y="80" class="l">AI ka jawab training, web search ya deep research se aata hai.</text>
    <text x="28" y="107" class="l">Jahan internet par data kam, wahan AI kamzor aur ghalat bhi.</text>
    <text x="28" y="139" class="l" font-weight="600">Is liye: achhi briefing do aur source check karo.</text>
  </g>

  <!-- ================= PART 2 ================= -->
  <rect x="815" y="315" width="745" height="745" rx="18" fill="#ecfdf5" stroke="#059669" stroke-width="3"/>
  <text x="837" y="360" class="h" fill="#059669">PART 2 · AI se baat kaise karein?</text>

  <g transform="translate(830,385)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#059669"/>
    <circle cx="40" cy="36" r="18" fill="#059669"/><text x="40" y="43" class="n">4</text>
    <text x="68" y="44" class="t">Context is the whole game</text>
    <text x="28" y="80" class="l">Context window, 6 layers: System prompt · Tools · Prompt ·</text>
    <text x="28" y="107" class="l">History · Files · Memory   |   Projects = context aik dafa</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Reading desk · Context rot → Reset, rescue nahi</text>
  </g>

  <g transform="translate(830,552)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#059669"/>
    <circle cx="40" cy="36" r="18" fill="#059669"/><text x="40" y="43" class="n">5</text>
    <text x="68" y="44" class="t">Reasoning (“think hard”)</text>
    <text x="28" y="80" class="l">Reasoning = jawab se pehle model ki apni working</text>
    <text x="28" y="107" class="l">Extended thinking: mushkil sawal ke liye · slow + mehnga</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Chhote kaam par thinking nahi · task length ~7 mahine double</text>
  </g>

  <g transform="translate(830,719)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#059669"/>
    <circle cx="40" cy="36" r="18" fill="#059669"/><text x="40" y="43" class="n">6</text>
    <text x="68" y="44" class="t">Sycophancy ka hal</text>
    <text x="28" y="80" class="l">Biased: find, defend, confirm, prove</text>
    <text x="28" y="107" class="l">Neutral: evaluate, compare, critique · “I don't know” allowed</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Rubric + 1–10 score · “There is always a next level”</text>
  </g>

  <g transform="translate(830,886)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#059669"/>
    <circle cx="40" cy="36" r="18" fill="#059669"/><text x="40" y="43" class="n">7</text>
    <text x="68" y="44" class="t">Brainstorm-iterate loop</text>
    <text x="28" y="80" class="l">Context → 3–5 options → feedback → repeat → aik expand</text>
    <text x="28" y="107" class="l">Outline before draft · ~9.5 par ruko · Diagnosis</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Brainstorm loose, Draft tight · apna jawab mat batao</text>
  </g>

  <!-- ================= PART 3 ================= -->
  <rect x="40" y="1090" width="745" height="580" rx="18" fill="#fff4ec" stroke="#ea580c" stroke-width="3"/>
  <text x="62" y="1135" class="h" fill="#ea580c">PART 3 · Text se aage</text>

  <g transform="translate(55,1160)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#ea580c"/>
    <circle cx="40" cy="36" r="18" fill="#ea580c"/><text x="40" y="43" class="n">8</text>
    <text x="68" y="44" class="t">Multimodal</text>
    <text x="28" y="80" class="l">Image: overall acha, detail kamzor · Diffusion = noise se image</text>
    <text x="28" y="107" class="l">[unclear] mark karwao · SVG → PNG → redraw · Audio meetings</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: AI 90% boring kaam, insaan 10% careful check</text>
  </g>

  <g transform="translate(55,1327)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#ea580c"/>
    <circle cx="40" cy="36" r="18" fill="#ea580c"/><text x="40" y="43" class="n">9</text>
    <text x="68" y="44" class="t">Aik prompt se app</text>
    <text x="28" y="80" class="l">Artifact (Claude) / Canvas (ChatGPT, Gemini)</text>
    <text x="28" y="107" class="l">Recipe: Goal · Input · Output   |   Mushkil: online multiplayer</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Aik screen + no accounts + no outside services = ban jayega</text>
  </g>

  <g transform="translate(55,1494)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#ea580c"/>
    <circle cx="40" cy="36" r="18" fill="#ea580c"/><text x="40" y="43" class="n">10</text>
    <text x="68" y="44" class="t">Data analysis</text>
    <text x="28" y="80" class="l">Code execution: andaza nahi, CALCULATOR</text>
    <text x="28" y="107" class="l">“Write and run code. Show me the code you ran.”</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Phir bhi check karo: totals, graph labels, ghalat column</text>
  </g>

  <!-- ================= PART 4 ================= -->
  <rect x="815" y="1090" width="745" height="580" rx="18" fill="#f5f0ff" stroke="#7c3aed" stroke-width="3"/>
  <text x="837" y="1135" class="h" fill="#7c3aed">PART 4 · Safe kaam aur sahi tool</text>

  <g transform="translate(830,1160)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#7c3aed"/>
    <circle cx="40" cy="36" r="18" fill="#7c3aed"/><text x="40" y="43" class="n">11</text>
    <text x="68" y="44" class="t">AI desktop apps (Cowork, OpenWork)</text>
    <text x="28" y="80" class="l">Task → Plan maango → Review/edit → Approve</text>
    <text x="28" y="107" class="l">Delete = recycle bin nahi · Chhota folder, full disk nahi</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Permission ladder · scope track record se barhta hai</text>
  </g>

  <g transform="translate(830,1327)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#7c3aed"/>
    <circle cx="40" cy="36" r="18" fill="#7c3aed"/><text x="40" y="43" class="n">12</text>
    <text x="68" y="44" class="t">Cost, speed, kaunsa model</text>
    <text x="28" y="80" class="l">Text &lt; Speech &lt; Images &lt; Video (~16x text)</text>
    <text x="28" y="107" class="l">Jagged · Model ladder · Arena monthly · 2 tabs khule</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Koi aik best model nahi · aik tool se shaadi mat karo</text>
  </g>

  <g transform="translate(830,1494)">
    <rect width="715" height="155" rx="14" fill="#fff"/><rect width="8" height="155" rx="4" fill="#7c3aed"/>
    <circle cx="40" cy="36" r="18" fill="#7c3aed"/><text x="40" y="43" class="n">13</text>
    <text x="68" y="44" class="t">Models checking models</text>
    <text x="28" y="80" class="l">Doosri FAMILY = alag blind spots (2 Claude = cross-check nahi)</text>
    <text x="28" y="107" class="l">Self-grade → 2nd family → critique wapas → 3rd family</text>
    <rect x="20" y="119" width="680" height="28" rx="8" fill="#fffbeb"/>
    <text x="30" y="139" class="y">Yaad: Score = progress, truth nahi · legal/medical = insaan expert</text>
  </g>

  <!-- ================= BOTTOM ================= -->
  <rect x="40" y="1700" width="745" height="360" rx="18" fill="#ffffff" stroke="#e3e6ee" stroke-width="2"/>
  <text x="62" y="1742" class="bh">13 sawal → 13 jawab</text>
  <text x="62" y="1776" class="bl">1. Kaise poochhun? → Briefing</text>
  <text x="62" y="1800" class="bl">2. AI ko pata kaise? → Training se</text>
  <text x="62" y="1824" class="bl">3. Training mein na ho? → Search / Deep research</text>
  <text x="62" y="1848" class="bl">4. Saamne kya rakhun? → Context</text>
  <text x="62" y="1872" class="bl">5. Mushkil sawal? → Think hard</text>
  <text x="62" y="1896" class="bl">6. Sach bolega? → Neutral wording + rubric</text>
  <text x="62" y="1920" class="bl">7. Behtar kaise? → Loop</text>
  <text x="430" y="1776" class="bl">8. Tasveer, awaaz? → Multimodal</text>
  <text x="430" y="1800" class="bl">9. Kuch banaye? → Artifact / Canvas</text>
  <text x="430" y="1824" class="bl">10. Hisaab sahi? → Code execution</text>
  <text x="430" y="1848" class="bl">11. Meri files? → Plan + approve</text>
  <text x="430" y="1872" class="bl">12. Kaunsa tool? → Cost, jagged, Arena</text>
  <text x="430" y="1896" class="bl">13. Kaun check kare? → Doosri family</text>
  <text x="430" y="1920" class="bl">        + insaan expert</text>
  <rect x="60" y="1950" width="705" height="88" rx="12" fill="#eef4ff"/>
  <text x="80" y="1984" class="bl" font-weight="600">Practice: sirf sawal dekho, jawab bolo,</text>
  <text x="80" y="2012" class="bl" font-weight="600">phir upar wale card se check karo.</text>

  <rect x="815" y="1700" width="745" height="360" rx="18" fill="#fffbeb" stroke="#f3d38a" stroke-width="2"/>
  <text x="837" y="1742" class="bh" fill="#b45309">Viva ki golden lines</text>
  <text x="837" y="1784" class="bl" font-weight="600">“A prompt is not a question, it is a briefing.”</text>
  <text x="837" y="1820" class="bl" font-weight="600">“Confidence is not correctness.”</text>
  <text x="837" y="1856" class="bl" font-weight="600">“Reset beats rescue.” (context rot)</text>
  <text x="837" y="1892" class="bl" font-weight="600">“There is always a next level.”</text>
  <text x="837" y="1928" class="bl" font-weight="600">“Write and run code. Show me the code you ran.”</text>
  <text x="837" y="1964" class="bl" font-weight="600">“Scope grows with track record.”</text>
  <text x="837" y="2000" class="bl" font-weight="600">“Models check each other for craft.</text>
  <text x="837" y="2026" class="bl" font-weight="600">  Humans check the facts that matter.”</text>
</svg>
