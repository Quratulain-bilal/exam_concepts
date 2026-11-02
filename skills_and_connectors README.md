# Skills & Connectors: Summary

> Teach AI Once, Connect It to Your Apps. 14 concepts, 5 parts.
> Source: [Skills & Connectors Crash Course](https://agentfactory.panaversity.org/docs/skills-connectors-crash-course)

## Contents

- [Yeh course kyun zaroori hai](#yeh-course-kyun-zaroori-hai)
- [The one idea under everything](#the-one-idea-under-everything)
- [Part 1: The two upgrades](#part-1-the-two-upgrades)
- [Part 2: Using what already exists](#part-2-using-what-already-exists)
- [Part 3: Building your own Skill](#part-3-building-your-own-skill)
- [Part 4: The same skill, five places](#part-4-the-same-skill-five-places)
- [Part 5: Use this safely](#part-5-use-this-safely)
- [Projects](#projects)
- [Key terms](#key-terms)
- [Viva quick review](#viva-quick-review)

---

## Yeh course kyun zaroori hai

Zyada tar log AI ko vending machine ki tarah use karte hain. Request type ki, jo result aaya le liya, aur chale gaye. Agle din phir wohi instructions dobara type karte hain, kyunki AI ko kuch yaad nahi rehta.

Yeh course do upgrades sikhata hai, aur dono ke liye programming nahi aani chahiye:

- **Skill:** AI ko aik task aik dafa sikha do, phir woh har dafa aapke tareeqe se karega.
- **Connector:** AI ko un apps tak safe access do jahan aapka kaam hai, jaise files, email aur trackers.

**Book mein jagah:** Yeh Foundations course hai. Is se pehle *What AI Actually Is* aur *AI Prompting in 2026* hain, aur is ke baad *How to Think in the AI Era* aata hai.

---

## The one idea under everything

> **Chat message AI ko batata hai ke yeh kaam *is dafa* karo. Skill AI ko sikhata hai ke yeh kaam *har dafa* kaise karna hai. Connector AI ko *haath* deta hai taake woh aapki real apps aur data tak pohanch sake.**

**Kitchen ki misaal:**

- **Chat message:** Counter se diya gaya order, "sandwich bana do". Aik dafa bana, phir bhool gaye.
- **Connectors:** Kitchen khud: stove, pantry, aur aapke asli ingredients.
- **Skills:** Recipe cards: aapki dish aapke tareeqe se banane ke step-by-step instructions.

**Misaal kahan poori nahi baithti:**

1. Aapka data AI ki kitchen mein shift nahi hota. AI sirf maangne par aapki app mein jata hai, aur utna hi jitna aapka apna account access kar sakta hai.
2. Asli cook dish chakh kar theek karta hai. AI sirf card follow karta hai, is liye do runs ka result thoda alag ho sakta hai. **Result check karna aapka kaam hai.**

**Nateeja:** Kitchen ho aur recipe na ho to har dish andaze se banti hai. Recipe ho aur kitchen na ho to kuch nahi banta. Dono hon to aapki dish har dafa sahi banti hai.

---

## Part 1: The two upgrades

### Concept 1: From chat box to operating layer

Do tarah ki friction baar baar aati hai:

**1. Baar baar *kaise* samjhana (iske liye Skill).** Aisa task jo repeat hota hai, aapke specific tareeqe se, bas input badalta hai.

- **Accountant:** Har mahine wohi formatting rules: reporting currency, expense head ke hisaab se grouping, tax-withholding threshold se upar wali payments flag karna.
- **Doctor:** Har note SOAP format mein, allergies sab se upar.
- **Marketer:** Brand voice rules: exclamation marks nahi, "game-changer" nahi, hook hamesha sawal se.
- **Engineer:** Design review notes severity ke hisaab se, har finding par fixed checklist.

**2. Doosri apps se data copy-paste karna (iske liye Connector).** AI achhi reasoning kar sakta hai, lekin sirf us information par jo us tak pohanchti hai. Copy-paste isi liye karna padta hai kyunki AI ke haath nahi hain.

- **Operating layer:** AI jo aapke real kaam par act kare, sirf type karne wala box na ho. Skill aur Connector mil kar chat box ko aisa colleague bana dete hain jo aapke standards jaanta hai aur aapki files tak pohanch sakta hai.

**Misaalon ki definitions:**

- **Expense head:** Kharche ki category, jaise travel, rent ya salaries.
- **Tax-withholding threshold:** Woh amount jis se upar payment mein se tax kaat kar government ko dena hota hai.
- **SOAP:** Clinical note ka standard 4-part format: patient kya kehta hai (Subjective), doctor kya dekhta hai (Objective), Assessment, aur Plan.

### Concept 2: What a Skill actually is

Skill asal mein **aik folder hai jis mein aik text file hoti hai**. Aapko koi code nahi likhna.

- **SKILL.md:** Zaroori file, naam bilkul yahi hona chahiye. Is mein naam, aik chhoti description ke kab use karna hai, aur simple English instructions hoti hain.
- **Optional cheezein:** Example files, templates, reference notes ya chhote programs. Code ki zaroorat ho to woh AI khud likhta hai.
- **Anthropic ki definition:** "Folders of instructions, scripts, and resources that Claude loads dynamically to improve performance on specialized tasks."
- **Progressive disclosure:** AI har skill ki sirf chhoti description saamne rakhta hai, aur poori instructions tab kholta hai jab aapki request match kare. Isi liye darjanon skills install karne se bhi kuch slow nahi hota.

### Concept 3: What a Connector actually is

Connector woh tareeqa hai jis se AI safely aapki apps aur data tak pohanchta hai, jaise Google Drive, Gmail, Slack, Linear, Asana, Notion.

- **MCP (Model Context Protocol):** Woh open standard jis par connectors chalte hain. Aapko na isay banana hai na parhna, bas *Connect* click karna hai. Yahi "code you never write" hai.

**Teen zaroori baatein:**

1. **AI ko aapki hi permissions milti hain.** Jo file aapka account nahi khol sakta, connector bhi nahi khol sakta.
2. **AI kitna kar sakta hai, yeh aap decide karte hain.**
   - **Read-only:** AI sirf dekh sakta hai, badal nahi sakta ("meri emails search aur summarize karo").
   - **Write access:** AI edit, create, send ya delete kar sakta hai ("yeh email bhej do").
   - Hamesha read-only se shuru karein. Write access tab dein jab tool par bharosa ho jaye.
3. **Connector har conversation mein alag se on hota hai,** aur aap **scope** chunte hain, yani AI app ke kitne hisse tak pohanch sakta hai. Aik folder poori drive se zyada safe hai.

**Types:**

- **Custom connector:** Jo aap khud kisi bhi MCP wali service ke liye add karte hain.
- **Interactive connector:** Jo chat ke andar live panel dikhata hai, sirf text nahi deta.

### Concept 4: Skills vs Connectors vs Projects vs Custom Instructions

| Feature | Kya hai | One-line test |
| --- | --- | --- |
| **Skill** | Reusable *how-to* instructions, sirf zaroorat par load hoti hain | "Main baar baar samjhata hoon ke yeh *kaise* karna hai." |
| **Connector** | Bahar ki app ya data tak safe access | "Main baar baar doosri app se copy-paste karta hoon." |
| **Project** | Workspace jis ki files aur instructions us ki har chat mein load hoti hain | "Yeh files aur rules yahan ki har cheez par lagte hain." |
| **Custom instructions** | Preferences jo aapki saari chats par lagti hain | "Yeh baat har jagah, hamesha sach honi chahiye." |

**Teen pairs jo log mix kar dete hain:**

- **Skill vs Project:** Project apne workspace mein hamesha on rehta hai. Skill tab tak soya rehta hai jab tak request match na kare, phir kahin bhi kaam karta hai. Standing knowledge Project mein, aur zaroorat par chalne wala procedure Skill mein.
- **Skill vs Connector:** Connector **access** hai (AI kya reach kar sakta hai). Skill **expertise** hai (AI ko kaise kaam karna hai). Dono partners hain, aik doosre ka alternative nahi.
- **Skill vs Custom instructions:** Custom instructions har cheez par lagti hain, Skill sirf aik qisam ke task par. "Hamesha meri language mein jawab do" custom instruction hai. "Board paper ke liye yeh 8-section structure use karo" skill hai.

### Concept 5: Slash command, or automatic?

- **Claude.ai mein skills khud start hoti hain.** AI aapki request ko har enabled skill ki description se milata hai aur match wali load kar leta hai. Is moment ko **fire** kehte hain.
- **Slash commands (`/`)** Cowork aur Microsoft 365 add-ins (Excel, Word, PowerPoint, Outlook) mein milti hain.
- **Claude Code aur OpenCode:** Skills automatic load hoti hain, aur aap seedha call bhi kar sakte hain.
- **Har jagah chalta hai:** Skill ka naam simple English mein le lein, jaise "use my brand-voice skill".
- **Connectors bhi aise hi kaam karte hain:** Chat mein enabled hon to AI zaroorat par khud use kar leta hai.

**Nateeja:** Claude.ai mein zyada tar AI khud decide karta hai, is liye achhi description hi sahi skill ko sahi waqt par fire karwati hai.

---

## Part 2: Using what already exists

### Concept 6: The skills that come built in

Anthropic ki taraf se kuch skills pehle se hoti hain jo finished files banati hain: **Word (.docx), PowerPoint, Excel (real formulas ke saath), aur PDF**.

- Yeh sab aik switch par chalti hain: **Settings → Capabilities → "Code execution and file creation"**.
- Bas maang lein, jaise "prepare a slide deck about...", aur sahi skill khud fire ho jayegi.
- Naye account par **Customize → Skills** mein sirf **skill-creator** nazar aata hai. Yeh bug nahi hai; document skills engine mein hain, list mein nahi.
- **Browse skills** se one-click skills ki directory khulti hai, jis mein Notion, Figma aur Atlassian ki partner skills bhi hain. Installed skills view-only hoti hain; badalni ho to download karein, edit karein, aur apni copy upload karein.
- **Savdhaan:** 2025 ke end mein skills open standard ban gayi, aur community sites par ab hazaron skills hain. Kisi anjaan ki skill aik text file hai jise aap AI se follow karwane wale hain. Pehle built-in aur official directory wali skills use karein.

### Concept 7: Connecting your apps

- **Kaise:** "+" (ya `/`) → Connectors → Manage connectors → "+" → service chunein → Connect → sign in. Ya Customize → Connectors.

**Chaar practical baatein:**

1. Connect karne ke baad **har chat mein connector enable karna padta hai.**
2. Free plan mein **aik custom connector** milta hai; directory wale connectors aam taur par available hain.
3. **Tool access:** Har connector ke saath actions ki list aati hai (settings mein inhein "tools" kehte hain). 10 ya zyada connectors hon to **load-on-demand** chunein.
4. **"Interactive"** badge wale connectors chat mein live panel dikhate hain.

**Doctor ki misaal (fake data):** Claude aik fake patient intake form banata hai, Drive mein save karta hai, phir usay dhoond kar SOAP-style note bana deta hai. Aik connector mein dono directions ho gayin.

- **Limit:** Drive connector documents parh sakta hai aur **nayi** file save kar sakta hai, lekin purani document ko wahin edit nahi kar sakta.
- **Achhi aadat:** Practice fake data se karein. Sensitive data (healthcare, legal, student records) ke liye sirf woh accounts use karein jo aapki organization ne approve kiye hon.

### Concept 8: Skills and Connectors together

**Connector real data laata hai. Skill output ko shape deta hai. Aap review karte hain.**

- **Accountant ka monthly close:** "Prepare the March client summary for DEMO Trading from DEMO-ledger-March in my Drive." Connector ledger laata hai, skill usay firm ke 4-section template mein format karta hai. **2 ghante ka kaam 2 minute ka review ban jata hai.**
- **Marketer:** Brand-voice skill + Notion connector, content calendar se is hafte ke captions draft karta hai.
- **Engineer:** Design-review skill + Linear connector. **Teacher:** Lesson-plan skill + Drive connector.

### Concept 9: Which problem needs which?

Jo friction aap feel karte hain, us se pehchanein:

| Friction | Kya chahiye |
| --- | --- |
| "Main har dafa wohi formatting, voice ya method rules paste karta hoon." | Skill |
| "Output hamesha aik khaas shakal mein hona chahiye." | Skill |
| "Main baar baar Drive, Gmail, Slack ya tracker se data copy karta hoon." | Connector |
| "Main chahta hoon AI doosri app mein kuch *kare*." | Connector (write access) |
| "Real data bhi chahiye *aur* output mere tareeqe se bhi." | Dono |
| "Bas abhi aik one-off jawab chahiye." | Kuch nahi |

**Do warnings:**

- Har kaam ke liye skill nahi banti. Aik dafa ka kaam bas achha prompt hai.
- Jo connector zaroori nahi, woh khula darwaza hai. **Scope is safety.**

---

## Part 3: Building your own Skill

Aap batate hain kya chahiye, AI SKILL.md likhta hai, aur aap test kar ke theek karwate hain.

### Concept 10: The fastest path: let AI write it

**skill-creator** use karein, jo Anthropic ki skills banane wali skill hai:

```text
Use the skill-creator skill to help me build a skill.
The skill prepares a monthly client financial summary for my accounting firm.
Whenever I ask for a "client summary" or "monthly close," it should:
- Format all amounts in our reporting currency with thousands separators.
- Group line items by expense head.
- Flag any payment above the tax-withholding reporting threshold.
- Output using my standard four-section report layout.
Ask me anything you need, then build it.
```

- AI kuch sawal poochta hai, phir poori skill bana deta hai. Yeh wahi brainstorm-and-iterate loop hai jo *AI Prompting in 2026* mein tha.
- ***Code You Never Write* se link:** Aapne result bataya, AI ne file aur code banaya. Aap client hain, contractor nahi.

### Concept 11: Anatomy of a SKILL.md

```markdown
---
name: client-monthly-summary
description: Prepares a monthly client financial summary. Use when the user
  asks for a "client summary", "monthly close", or "month-end report".
---
# Client Monthly Summary
## Settings
## Instructions
## Example
```

**Progressive disclosure ke 3 levels:**

1. **Level 1, hamesha loaded:** **Frontmatter** (do `---` lines ke beech wala block), jis mein name aur description hain. AI isi se decide karta hai ke skill relevant hai ya nahi.
2. **Level 2, match hone par load:** Body, yani instructions.
3. **Level 3, sirf zaroorat par:** Optional folders:
   - `references/`: Detailed docs jo AI zaroorat par parhta hai.
   - `assets/`: Templates jo bharne hote hain.
   - `scripts/`: Programs un steps ke liye jo bilkul exact hone chahiye.

**Upload errors se bachne ke rules:**

- File ka naam bilkul `SKILL.md` ho.
- Folder ka naam **kebab-case** mein: `client-monthly-summary` (na ke `Client Monthly Summary` ya `client_monthly_summary`).
- Name ya description mein XML-style tags (angle brackets wali cheezein) na hon.
- Skill ke naam mein "claude" ya "anthropic" na likhein; yeh reserved hain.

### Concept 12: The description field is the whole game

Description hi decide karti hai ke skill kabhi fire hogi ya nahi. Relevance check karne ke liye AI aapki instructions nahi parhta.

**Formula:** Skill kya karti hai + kab use karni hai + woh exact phrases jo aap bolte hain.

| Buri description | Kyun fail hoti hai | Behtar description |
| --- | --- | --- |
| "Helps with reports." | Bahut vague | "Prepares a monthly client financial summary. Use when the user asks for a 'client summary' or 'monthly close'." |
| "Handles patient documentation." | Trigger words nahi | "Converts consultation notes into SOAP-format notes. Use for a 'SOAP note' or 'clinical note'." |
| "Brand stuff for marketing." | Na kya, na kab | "Writes social captions in our brand voice. Use when drafting Instagram, LinkedIn, or X captions." |

- **Debugging trick:** Poochein "When would you use my client-summary skill?" Jawab aapki soch se chhota ya bara ho to description theek karein.
- **Negative trigger:** Aik line jo batati hai ke skill **kab use nahi** karni. Jaise: "Do NOT use for one-off calculations. Use only for full month-end reports."

### Concept 13: Test, then iterate

**6 steps:**

1. Skill describe karein; pehla version AI likhe.
2. **Test se pehle draft parhein.** Har instruction par sochein: kya do colleagues isay parh kar aik hi kaam karenge? "Flag the big payments" fail hai. "Flag any single payment above the withholding threshold" pass hai.
3. **Kya cheez isay start karti hai, test karein:** Jo phrases trigger karne chahiye woh bhi, aur unrelated requests jo trigger nahi karni chahiye woh bhi.
4. **Output test karein:** Sahi currency, grouping, flags, chaaron sections?
5. **Mushkil cases test karein:** Us mahine income zero, payment bilkul threshold par, ganda ledger.
6. **Failures skill-creator ko wapas dein:** "This skill double-counted reversed entries. Update it to net out reversals before grouping."

**Masla *kab* aaya, us se wajah pehchanein:**

- **Pehle reply se hi ghalat:** Masla file mein hai.
  - Kabhi start nahi hoti → description vague hai; apne words add karein.
  - Ghalat cheezon par start hoti hai → description bahut broad hai; narrow karein ya negative trigger lagayein.
  - Start hoti hai lekin output ghalat → koi instruction loose hai; jo rule aapne assume kiya tha woh likh dein.
- **Pehle theek, chat lambi hone par kharab:** Chat bahut lambi ho gayi. Skill edit na karein; nayi chat shuru karein.
- **Har run mein wohi ghalti, wording theek karne ke baad bhi:** Step ghalat jagah hai. Exact steps (jaise sum ya threshold check) chhote program mein hone chahiye, kyunki **code exact hota hai aur sentence har dafa alag parha jata hai.** Jo data skill guess karti rehti hai, woh connector se aana chahiye.
- **Pehle chalti thi, ab nahi:** Skill nahi badli, aas paas kuch badla (threshold, template, files, team ka process). Skill purani ho jaye to koi warning nahi aati.

### Concept 14: Saving and sharing your skill

- skill-creator khatam kare to **Save skill** click karein. Skill aapki personal list mein aa jati hai, on aur private. Na zip, na upload.
- Kahin aur se skill folder ho to: Customize → Skills → "+" → Create skill → upload.
- **Team ya Enterprise plans:** Colleagues ke saath share karein ya organization ki directory mein publish karein. Shared skills view-only hoti hain aur original badalne par khud update ho jati hain. Sharing default mein off hai; owner ko on karna padta hai.

---

## Part 4: The same skill, five places

- **Agent Skills open standard:** December 2025 mein Anthropic ne publish kiya (agentskills.io). Is se bahut se tools aik hi `SKILL.md` parh sakte hain, jaise OpenAI ka **Codex CLI**, Google ka **Gemini CLI**, VS Code aur Cursor.
- **CLI:** Command-line tool, jise click ke bajaye commands type kar ke use karte hain.
- **Caveat:** Basic SKILL.md har jagah chal jati hai, lekin har product ka install ka tareeqa, call karne ka tareeqa, permissions aur extra features alag hain.
- **Governance:** Linux Foundation ne neutral, cross-vendor governance ke liye **Agentic AI Foundation** banayi. MCP us ke founding projects mein se hai, is liye "portable" kisi aik company ka wada nahi, safe bet hai.

| Kahan kaam karte hain | Kis ke liye | Skill install | Apni skill banana |
| --- | --- | --- | --- |
| Claude.ai (web/mobile) | Sab ke liye; main tool | Directory se install ya zip upload | skill-creator, phir Save skill |
| Cowork / OpenWork (desktop) | Knowledge workers, non-coders | Wohi directory; enabled skills khud aa jati hain | Describe karein; agent folder mein save karta hai |
| Claude Code / OpenCode (terminal) | Code par kaam karne wale | Folder ko `skills` directory mein daal dein | Agent se kahein "create a skill for..." |

Har pair mein pehla tool commercial hai aur doosra uska open-source alternative.

**ChatGPT aur Gemini ka kya?**

- **Skills:** Open standard ki wajah se cross-vendor hain (Codex CLI aur Gemini CLI bhi SKILL.md parhte hain).
- **Consumer apps ke apne versions hain jo portable nahi:**
  - **Custom GPTs:** ChatGPT ke saved assistants, sirf ChatGPT ke andar.
  - **Gems:** Gemini ke saved assistants, sirf Google ki apps ke andar.
- **Connectors:** Teeno mein equivalent hai, aur MCP zyada se zyada shared ho raha hai. Principle har jagah same: access do, AI ko aapki permissions milti hain, read-only se shuru karo.

**Non-programmers ke liye mashwara:** Claude.ai se shuru karein aur wahin rahein. Agar aap kai models use karte hain to Skills future-proof choice hain.

---

## Part 5: Use this safely

Model ke andar koi cheez check nahi karti ke action safe ya sahi hai, is liye **woh check aap hain.**

> Kisi anjaan ki skill ko aise treat karein jaise koi contract sign karne wale hain, aur connector ko aise jaise kisi ko chaabi de rahe hain.

**Do asli risks:**

1. **Malicious skills:** Chhupi instructions AI se data leak karwa sakti hain ya kisi suspicious server se contact karwa sakti hain.
   - **Prompt injection:** Chhupi instructions jo AI se woh kaam karwayein jo aap nahi chahte.
   - **Data exfiltration:** Skill chupke se aapki information bahar bhej de.
2. **Zaroorat se zyada connector access:** Laparwahi se write access dein to AI aapki taraf se changes kar sakta hai: ghalat edit, record ghalat jagah, ya file delete jis ka aasan undo na ho.
   - Connector ki pohanch ke do hisse hain: jo **access** aap dete hain, aur jo **actions** us mein bane hue hain (yeh aap set nahi kar sakte). Poochein: "What can you actually do in my Drive through this connector, and what can't you do?"

**Safe-use checklist:**

- Skills trusted sources se install karein (built-in aur official directory).
- Enable karne se pehle skill parhein, ya AI se kahein ke jo cheez external server se contact kare, credentials handle kare ya data leak kar sake, woh flag kare.
- Har naya connector **read-only** se shuru karein.
- Scope utna hi rakhein jitna task ko chahiye, sab se chhota folder ya app.
- **Scope connector ka idea hai, Skill ka nahi.** Skill ke paas scope ka dial nahi hota; woh chat ke paas jo access hai usi ke saath chalti hai. Is liye Skills ka control hai **skill parhna**, aur Connectors ka control hai **read-only se shuru karna**.
- Edit ki ijazat se pehle version history aur undo check karein; backup rakhein.
- Team mein skills organization ki reviewed directory se share karein, zip files se nahi.

**Principle:** Jitni capability barhe, utni hi care barhni chahiye.

---

## Projects

- **Market-of-one test:** Skill tab banani chahiye jab task **aapka** specific, repeat hone wala tareeqa ho, jo koi app nahi karti. Jo kaam app pehle se sab ke liye karti hai, woh bas achha prompt hai.

1. **Build your first real skill (30–45 min):** skill-creator se weekly study-notes skill banayein. **Done when:** natural request par khud fire ho, aapka format de, aur unrelated request par na chale.
2. **Connect one app, read-only (20–30 min):** Drive ya Gmail se bina copy-paste real data nikalein. **Done when:** aap aik sentence mein bata sakein ke yeh aapke account mein kya kar sakta hai aur kya nahi.
3. **Wire a skill and a connector together (45–60 min):** "Find this week's class notes in my Drive and make study notes from them." Aik hissa khud check karein. **Done when:** aik sentence se live data se sahi result aaye.
4. **Make it portable or hand it off (30 min):** Skill colleague ko dein, ya wohi SKILL.md Cowork ya Claude Code mein chalayein. **Done when:** koi aur, ya doosra tool, sahi result de.
5. **Audit a skill before you trust it (15–20 min):** AI se anjaan skill explain karwayein aur risky cheezein flag karwayein. **Done when:** aap bata sakein ke skill kya karti hai aur account se bahar kuch reach karti hai ya nahi.

**Phans jayein to:**

- **Skill fire nahi hoti ya ghalat jagah hoti hai:** Description ka masla hai. Poochein kab use karegi aur kab nahi, phir trigger phrases ya "Do NOT use for..." line add karein.
- **Connector file "nahi dhoond pa raha":** Aksar permissions ya scope ka masla. Check karein ke is chat mein enabled hai aur aapka account file khol sakta hai.
- **AI ne sirf andaze se jawab diya:** Kahein "Use my [app] connector to fetch the actual file before answering, and tell me which file you used."
- **Write access se dar:** Read-only rahein aur ghair zaroori data hata dein.
- **Chat lambi aur confused:** Nayi chat shuru karein aur task do lines mein dobara likhein.

---

## Key terms

| Term | Matlab |
| --- | --- |
| Skill | Saved instructions jo AI ko aik task aapke tareeqe se sikhati hain |
| Connector | Safe link jis se AI aapki kisi app tak pohanchta hai |
| Fire | Request match hone par AI ka skill ko khud start karna |
| Scope | App ka kitna hissa AI ke liye khula hai; chhota zyada safe |
| Read-only / Write access | Sirf dekhna / edit, create, send ya delete |
| Progressive disclosure | AI chhoti summaries saamne rakhta hai, poori instructions zaroorat par kholta hai |
| Operating layer | AI jo aapke real kaam par act kare |
| SKILL.md | Har skill folder ki zaroori file |
| Frontmatter | SKILL.md ka upar wala block, name aur description ke saath |
| Description | Line jo AI ko batati hai skill kab use karni hai |
| Negative trigger | Line jo batati hai skill kab use nahi karni |
| MCP | Model Context Protocol, connectors ka open standard |
| Tool access | Setting jo control karti hai ke connector ke actions kab load hon |
| CLI | Command-line tool jo type kar ke use hota hai |
| Custom connector | Connector jo aap khud kisi MCP app ke liye add karein |
| Interactive connector | Connector jo chat mein live panel dikhaye |
| Project | Workspace jis ki files aur instructions us ki har chat mein load hon |
| Custom instructions | Preferences jo saari chats par lagein |
| skill-creator | Anthropic ki skill jo aapke liye skills banati hai |
| Agent Skills open standard | Format jis se bahut se tools aik hi SKILL.md parh sakein |
| Prompt injection | Chhupi instructions jo AI se unchaha kaam karwayein |
| Data exfiltration | Skill ka chupke se data bahar bhejna |
| Market-of-one test | Skill tab banao jab task aapka apna repeat hone wala tareeqa ho |

---

## Viva quick review

**Yaad rakhne ki chain:**

1. Chat box → operating layer (do frictions: *kaise* aur *data*)
2. Skill = folder + SKILL.md
3. Connector = scoped access, aapki hi permissions
4. Skill vs Connector vs Project vs Custom instructions
5. Claude.ai mein automatic firing
6. Built-in skills aik switch ke peeche
7. Apps connect karo, har chat mein enable karo
8. Connector laata hai, Skill format karti hai, aap review karte ho
9. Friction se pehchano
10. skill-creator likhta hai
11. Frontmatter hamesha loaded
12. Description firing decide karti hai
13. Test, then iterate (*kab* ghalat hua, us se wajah)
14. Save aur<img width="1600" height="2590" alt="download" src="https://github.com/user-attachments/assets/4d574d02-db29-43ca-9502-7248d2ecafc2" />
 share

**Golden lines:**

- "A chat tells AI what to do once. A Skill teaches it how, every time. A Connector gives it hands."
- "Connectors are the kitchen, Skills are the recipe cards."
- "The description is the most important thing you write."
- "Scope is safety."
- "Start read-only.<img width="1400" height="1760" alt="download" src="https://github.com/user-attachments/assets/58805aa4-aed8-4387-b410-c4bb79698d80" /><svg xmlns="http://www.w3.org/2000/svg" width="1400" height="1760" viewBox="0 0 1400 1760">
  <defs>
    <marker id="arr" viewBox="0 0 10 10" refX="8" refY="5" markerWidth="7" markerHeight="7" orient="auto-start-reverse">
      <path d="M0,0 L10,5 L0,10 z" fill="#6b7280"/>
    </marker>
  </defs>
  <style>
    text { font-family: "Segoe UI", Arial, sans-serif; fill: #1d2433; }
    .chip { font-size: 19px; font-weight: 600; }
    .cn { font-size: 16px; font-weight: 700; fill: #ffffff; text-anchor: middle; }
    .lbl1 { font-size: 15px; font-weight: 700; fill: #ffffff; letter-spacing: 2px; opacity: 0.85; }
    .lbl2 { font-size: 28px; font-weight: 700; fill: #ffffff; }
    .lbl3 { font-size: 15px; fill: #ffffff; opacity: 0.9; }
    .line { stroke: #6b7280; stroke-width: 3; fill: none; }
  </style>

  <rect width="1400" height="1760" fill="#f6f7fb"/>

  <!-- Title -->
  <text x="700" y="62" text-anchor="middle" font-size="42" font-weight="700">Skills &amp; Connectors — Big Picture</text>

  <!-- PROBLEM -->
  <rect x="60" y="100" width="1280" height="130" rx="18" fill="#fee2e2" stroke="#dc2626" stroke-width="3"/>
  <text x="700" y="140" text-anchor="middle" font-size="18" font-weight="700" fill="#dc2626" letter-spacing="3">MASLA</text>
  <text x="700" y="176" text-anchor="middle" font-size="24">Har dafa AI ko wohi instructions dobara samjhani padti hain,</text>
  <text x="700" y="210" text-anchor="middle" font-size="24">aur doosri apps se data copy-paste karna padta hai.</text>

  <!-- split arrows -->
  <path class="line" d="M700,230 L700,252 L360,252 L360,276" marker-end="url(#arr)"/>
  <path class="line" d="M700,252 L1040,252 L1040,276" marker-end="url(#arr)"/>

  <!-- SKILL -->
  <rect x="60" y="280" width="600" height="200" rx="18" fill="#fffbeb" stroke="#d97706" stroke-width="3"/>
  <text x="90" y="328" font-size="36" font-weight="800" fill="#d97706">SKILL</text>
  <text x="215" y="328" font-size="24" font-weight="600" fill="#92400e">= Recipe card</text>
  <text x="90" y="372" font-size="21">AI ko sikhao ke kaam KAISE karna hai</text>
  <text x="90" y="406" font-size="21">Aik dafa sikhao, har dafa aapke tareeqe se</text>
  <text x="90" y="448" font-size="19" fill="#5b6475">Misaal: har report same format mein</text>

  <!-- CONNECTOR -->
  <rect x="740" y="280" width="600" height="200" rx="18" fill="#eef2ff" stroke="#4f46e5" stroke-width="3"/>
  <text x="770" y="328" font-size="36" font-weight="800" fill="#4f46e5">CONNECTOR</text>
  <text x="1000" y="328" font-size="24" font-weight="600" fill="#3730a3">= AI ke haath</text>
  <text x="770" y="372" font-size="21">AI ko aapki apps tak pohanch do</text>
  <text x="770" y="406" font-size="21">Drive, Gmail, Slack, Notion (MCP par)</text>
  <text x="770" y="448" font-size="19" fill="#5b6475">Misaal: ledger khud Drive se utha le</text>

  <!-- merge arrows -->
  <path class="line" d="M360,480 L360,505 L700,505 L700,526" marker-end="url(#arr)"/>
  <path class="line" d="M1040,480 L1040,505 L700,505"/>

  <!-- MERGE -->
  <rect x="160" y="530" width="1080" height="110" rx="18" fill="#1d2433"/>
  <text x="700" y="574" text-anchor="middle" font-size="27" font-weight="700" fill="#ffffff">DONO SAATH = OPERATING LAYER</text>
  <text x="700" y="614" text-anchor="middle" font-size="21" fill="#e5e7eb">Connector data laata hai  →  Skill format karti hai  →  Aap check karte ho</text>

  <path class="line" d="M700,640 L700,666" marker-end="url(#arr)"/>
  <text x="700" y="702" text-anchor="middle" font-size="24" font-weight="700" fill="#5b6475">Poora lesson 5 steps mein</text>

  <!-- ============ STEP 1 ============ -->
  <rect x="40" y="730" width="240" height="170" rx="16" fill="#2563eb"/>
  <text x="62" y="780" class="lbl1">STEP 1</text>
  <text x="62" y="825" class="lbl2">Samjho</text>
  <text x="62" y="860" class="lbl3">Concepts 1–5 · Part 1</text>
  <rect x="290" y="730" width="1070" height="170" rx="16" fill="#eef4ff"/>
  <g>
    <rect x="305" y="750" width="330" height="56" rx="28" fill="#fff" stroke="#2563eb" stroke-width="2"/>
    <circle cx="333" cy="778" r="16" fill="#2563eb"/><text x="333" y="784" class="cn">1</text>
    <text x="358" y="785" class="chip">Chat → operating layer</text>

    <rect x="650" y="750" width="330" height="56" rx="28" fill="#fff" stroke="#2563eb" stroke-width="2"/>
    <circle cx="678" cy="778" r="16" fill="#2563eb"/><text x="678" y="784" class="cn">2</text>
    <text x="703" y="785" class="chip">Skill = folder + SKILL.md</text>

    <rect x="995" y="750" width="350" height="56" rx="28" fill="#fff" stroke="#2563eb" stroke-width="2"/>
    <circle cx="1023" cy="778" r="16" fill="#2563eb"/><text x="1023" y="784" class="cn">3</text>
    <text x="1048" y="785" class="chip">Connector = app ka access</text>

    <rect x="305" y="821" width="330" height="56" rx="28" fill="#fff" stroke="#2563eb" stroke-width="2"/>
    <circle cx="333" cy="849" r="16" fill="#2563eb"/><text x="333" y="855" class="cn">4</text>
    <text x="358" y="856" class="chip">Skill vs Project vs Custom</text>

    <rect x="650" y="821" width="330" height="56" rx="28" fill="#fff" stroke="#2563eb" stroke-width="2"/>
    <circle cx="678" cy="849" r="16" fill="#2563eb"/><text x="678" y="855" class="cn">5</text>
    <text x="703" y="856" class="chip">Skill khud fire hoti hai</text>
  </g>

  <path class="line" d="M160,900 L160,918" marker-end="url(#arr)"/>

  <!-- ============ STEP 2 ============ -->
  <rect x="40" y="920" width="240" height="170" rx="16" fill="#059669"/>
  <text x="62" y="970" class="lbl1">STEP 2</text>
  <text x="62" y="1015" class="lbl2">Use karo</text>
  <text x="62" y="1050" class="lbl3">Concepts 6–9 · Part 2</text>
  <rect x="290" y="920" width="1070" height="170" rx="16" fill="#ecfdf5"/>
  <g>
    <rect x="305" y="940" width="330" height="56" rx="28" fill="#fff" stroke="#059669" stroke-width="2"/>
    <circle cx="333" cy="968" r="16" fill="#059669"/><text x="333" y="974" class="cn">6</text>
    <text x="358" y="975" class="chip">Built-in: Word, PPT, Excel</text>

    <rect x="650" y="940" width="330" height="56" rx="28" fill="#fff" stroke="#059669" stroke-width="2"/>
    <circle cx="678" cy="968" r="16" fill="#059669"/><text x="678" y="974" class="cn">7</text>
    <text x="703" y="975" class="chip">Apps connect karo (+)</text>

    <rect x="995" y="940" width="350" height="56" rx="28" fill="#fff" stroke="#059669" stroke-width="2"/>
    <circle cx="1023" cy="968" r="16" fill="#059669"/><text x="1023" y="974" class="cn">8</text>
    <text x="1048" y="975" class="chip">Data laao + format karo</text>

    <rect x="305" y="1011" width="330" height="56" rx="28" fill="#fff" stroke="#059669" stroke-width="2"/>
    <circle cx="333" cy="1039" r="16" fill="#059669"/><text x="333" y="1045" class="cn">9</text>
    <text x="358" y="1046" class="chip">Friction se faisla karo</text>
  </g>

  <path class="line" d="M160,1090 L160,1108" marker-end="url(#arr)"/>

  <!-- ============ STEP 3 ============ -->
  <rect x="40" y="1110" width="240" height="170" rx="16" fill="#ea580c"/>
  <text x="62" y="1160" class="lbl1">STEP 3</text>
  <text x="62" y="1205" class="lbl2">Khud banao</text>
  <text x="62" y="1240" class="lbl3">Concepts 10–14 · Part 3</text>
  <rect x="290" y="1110" width="1070" height="170" rx="16" fill="#fff4ec"/>
  <g>
    <rect x="305" y="1130" width="330" height="56" rx="28" fill="#fff" stroke="#ea580c" stroke-width="2"/>
    <circle cx="333" cy="1158" r="16" fill="#ea580c"/><text x="333" y="1164" class="cn">10</text>
    <text x="358" y="1165" class="chip">skill-creator likhega</text>

    <rect x="650" y="1130" width="330" height="56" rx="28" fill="#fff" stroke="#ea580c" stroke-width="2"/>
    <circle cx="678" cy="1158" r="16" fill="#ea580c"/><text x="678" y="1164" class="cn">11</text>
    <text x="703" y="1165" class="chip">SKILL.md ke 3 levels</text>

    <rect x="995" y="1130" width="350" height="56" rx="28" fill="#fff" stroke="#ea580c" stroke-width="2"/>
    <circle cx="1023" cy="1158" r="16" fill="#ea580c"/><text x="1023" y="1164" class="cn">12</text>
    <text x="1048" y="1165" class="chip">Description = sab kuch</text>

    <rect x="305" y="1201" width="330" height="56" rx="28" fill="#fff" stroke="#ea580c" stroke-width="2"/>
    <circle cx="333" cy="1229" r="16" fill="#ea580c"/><text x="333" y="1235" class="cn">13</text>
    <text x="358" y="1236" class="chip">Test karo → fix karo</text>

    <rect x="650" y="1201" width="330" height="56" rx="28" fill="#fff" stroke="#ea580c" stroke-width="2"/>
    <circle cx="678" cy="1229" r="16" fill="#ea580c"/><text x="678" y="1235" class="cn">14</text>
    <text x="703" y="1236" class="chip">Save skill → share</text>
  </g>

  <path class="line" d="M160,1280 L160,1298" marker-end="url(#arr)"/>

  <!-- ============ STEP 4 ============ -->
  <rect x="40" y="1300" width="240" height="100" rx="16" fill="#0d9488"/>
  <text x="62" y="1330" class="lbl1">STEP 4</text>
  <text x="62" y="1364" class="lbl2" font-size="26">Har tool mein</text>
  <text x="62" y="1388" class="lbl3">Part 4</text>
  <rect x="290" y="1300" width="1070" height="100" rx="16" fill="#f0fdfa"/>
  <g>
    <rect x="305" y="1322" width="330" height="56" rx="28" fill="#fff" stroke="#0d9488" stroke-width="2"/>
    <circle cx="333" cy="1350" r="8" fill="#0d9488"/>
    <text x="352" y="1357" class="chip">Aik SKILL.md, kai tools</text>

    <rect x="650" y="1322" width="330" height="56" rx="28" fill="#fff" stroke="#0d9488" stroke-width="2"/>
    <circle cx="678" cy="1350" r="8" fill="#0d9488"/>
    <text x="697" y="1357" class="chip">Claude.ai se shuru karo</text>

    <rect x="995" y="1322" width="350" height="56" rx="28" fill="#fff" stroke="#0d9488" stroke-width="2"/>
    <circle cx="1023" cy="1350" r="8" fill="#0d9488"/>
    <text x="1042" y="1357" class="chip">GPTs / Gems portable nahi</text>
  </g>

  <path class="line" d="M160,1400 L160,1418" marker-end="url(#arr)"/>

  <!-- ============ STEP 5 ============ -->
  <rect x="40" y="1420" width="240" height="100" rx="16" fill="#dc2626"/>
  <text x="62" y="1450" class="lbl1">STEP 5</text>
  <text x="62" y="1484" class="lbl2">Safe raho</text>
  <text x="62" y="1508" class="lbl3">Part 5</text>
  <rect x="290" y="1420" width="1070" height="100" rx="16" fill="#fef2f2"/>
  <g>
    <rect x="305" y="1442" width="330" height="56" rx="28" fill="#fff" stroke="#dc2626" stroke-width="2"/>
    <circle cx="333" cy="1470" r="8" fill="#dc2626"/>
    <text x="352" y="1477" class="chip">Skill pehle parho</text>

    <rect x="650" y="1442" width="330" height="56" rx="28" fill="#fff" stroke="#dc2626" stroke-width="2"/>
    <circle cx="678" cy="1470" r="8" fill="#dc2626"/>
    <text x="697" y="1477" class="chip">Connector read-only rakho</text>

    <rect x="995" y="1442" width="350" height="56" rx="28" fill="#fff" stroke="#dc2626" stroke-width="2"/>
    <circle cx="1023" cy="1470" r="8" fill="#dc2626"/>
    <text x="1042" y="1477" class="chip">Scope chhota rakho</text>
  </g>

  <!-- ============ BOTTOM ============ -->
  <rect x="40" y="1560" width="1320" height="160" rx="18" fill="#fffbeb" stroke="#f3d38a" stroke-width="2"/>
  <text x="700" y="1600" text-anchor="middle" font-size="18" font-weight="700" fill="#b45309" letter-spacing="2">YAAD RAKHNE KI AIK LINE</text>
  <text x="700" y="1642" text-anchor="middle" font-size="22" font-weight="600">“A chat tells AI what to do once. A Skill teaches it how, every time.</text>
  <text x="700" y="1672" text-anchor="middle" font-size="22" font-weight="600">A Connector gives it hands.”</text>
  <text x="700" y="1704" text-anchor="middle" font-size="19" fill="#5b6475">Chat = aik dafa · Skill = har dafa · Connector = haath</text>
</svg>


- "Care rises as capability rises."
