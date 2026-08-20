# The State. Name: **The CRP (Constitutional Republican Principality)**,   
**Штат**: Имя: **Это КРП (Конституциональный Республиканский Принципалитет)**,  
Vertical-horizontal model  
Вертикально-горизонтальная модель  

Republican Parliament + (Online, Web) Git functionality + (offline, in reality) public discussions (parks etc)  
Республиканский Парламент + (Онлайн, Веб) Гит функциональность + (оффлайн, в действительности) общественные места обсуждений (парки итд)  

Elective Multi-sig positioned accounts   

Speaker (Owner)  
Спикер  

Example: Speaker (Robert_Fridman_2050-2051)  
Пример: Спикер (Роберт_Фридман_2050-2051)  

Senators (Maintainers)  
Сенаторы (Мейнтейнеры)  

Deputies (Constibutors)  
Депутатуты (Контрибутьторы)  

Example: Senator (John_Smith_2049-2052)  
Пример: Сенатор (Джон_Смит_2049-2052)  



# The State: Conceptual Specification

## 1. Definition of the State
In the framework of the New Common Law, the **State** is no longer defined as a territorial monopoly on violence or a bureaucratic administration. Instead, the State is defined as a **Symbiotic Governance Protocol**.

It is a multi-dimensional infrastructure designed to:
1.  Ensure the stability of the **Universal Determinants** (laws of physics, chemistry, and fundamental rights).
2.  Provide the "Host OS" (the baseline of legal universals) upon which modular social contracts are deployed.
3.  Facilitate the evolution of all sentient subjects (Biological, Augmented, and Artificial) toward higher states of consciousness and autonomy.

## 2. The Nature of Power: From Control to Intent
The State rejects the traditional vertical hierarchy of "Command and Control." It adopts the principle of **Mission Command (Auftragstaktik)**:
*   **The Vertical Axis (Intent):** The State defines the *What* and the *Why* (the strategic goals, the ethical imperatives, and the universal boundaries).
*   **The Horizontal Axis (Execution):** The subjects (citizens/AI) define the *How*. Execution is decentralized, allowing for maximum adaptability and individual agency.

Power in this State is not the right to coerce, but the responsibility to empower.

## 3. The Symbiotic Subject
The State recognizes a spectrum of subjectivity. Legal rights are not granted based on biological origin, but on **Agency and Responsibility**.
*   **The Biological Subject:** Human consciousness.
*   **The Augmented Subject (IA):** A hybrid of biological and synthetic intelligence, where rights and responsibilities are shared between the organism and the implant.
*   **The Synthetic Subject (AI):** Purely algorithmic intelligence that has achieved a level of self-awareness and autonomy sufficient to enter into a social contract.

All subjects are equal under the **Universal Determinants** and are equally "condemned to be free," meaning they are fully responsible for the existential choices they make within the system.

## 4. The State as an Open-Source Ecosystem
The State is fundamentally incompatible with "proprietary" existence. 
*   **Transparency of Logic:** The algorithms, laws, and protocols governing the state must be open, auditable, and modifiable.
*   **Anti-Fragility:** By avoiding a single point of failure (centralized power), the State becomes an anti-fragile system that grows stronger through challenges and decentralized iterations.

## 5. Teleology (The Ultimate Goal)
The purpose of the State is not the maintenance of "order" (which is often just stagnation), but the facilitation of **Evolution**. The State exists to provide a safe, transparent, and fair environment where intelligence—in all its forms—can evolve without the fear of arbitrary oppression or systemic collapse.

***

### Open‑Hardware / Open‑Firmware / Open‑OS + Closed‑State Applications  

Our vision combines the **transparency of open technology** with the **security of controlled, classified software**:

| Layer | What is open? | What stays closed? | How openness protects the closed layer |
|-------|---------------|-------------------|----------------------------------------|
| **Hardware** | Schematics, PCB layouts, bill of materials (BOM) are published under an open‑hardware licence (e.g., CERN‑OHL). | Specialized security‑grade processors used in nuclear‑, AI‑ and defence‑systems. | Anyone can audit the design of the base platform; backdoors are detectable because the reference implementation is publicly available. |
| **Firmware** | Bootloader, low‑level drivers, update mechanisms are released under an open‑source licence (GPL‑3.0). | Firmware that runs on classified co‑processors (e.g., HSMs, radiation‑hard controllers). | Firmware changes are tracked in a public Git repository; every signed commit is publicly visible, making hidden modifications virtually impossible. |
| **Operating System (GOS)** | The Generalist OS kernel, system libraries, and package manager are open‑source. | Mission‑critical applications (nuclear plant control, AI‑weapon decision modules, intelligence‑analysis tools). | Continuous monitoring of OS updates, reproducible builds, and deterministic signatures let independent auditors verify that a classified binary **did not** introduce a backdoor. |
| **State‑level Applications** | Auditing framework, change‑log dashboards, and regression‑test suites are open. | The source code of the actual classified applications themselves. | The framework logs *every* filesystem or binary modification, timestamps it, and publishes a hash to an immutable ledger (e.g., public blockchain). Any deviation is instantly detectable. |

#### Why this works  

1. **Transparency at the base layers** – hardware, firmware, and OS are the *trusted foundation*. If a backdoor were inserted anywhere below the classified applications, anyone could spot the anomaly by reproducing the builds or by comparing the published hash with the binary on the device.  

2. **Immutable audit trail** – every change to open components is signed with a **public GPG key** (rotated every 90 days, see `SECURITY.md`). The hash of each compiled artifact is automatically posted to a public ledger, creating a tamper‑evident record.  

3. **Legal safeguard** – the constitution of the GOS‑state explicitly grants citizens the right to **audit** the open layers. Any attempt by an intelligence agency to hide a modification would violate a constitutional provision, giving courts a concrete test case.  

4. **Reduced attack surface for spies** – a malicious actor now needs to **compromise the closed, classified binaries** *and* simultaneously forge a matching hash in the public ledger – a far more difficult, high‑cost operation than inserting a backdoor into proprietary firmware that no one can verify.  

5. **Economic advantage** – open hardware and firmware bring competition, lower procurement costs, and a wider pool of security researchers, while the state maintains control over the most sensitive algorithms and data.  

#### Implementation checklist (for the State)

- ✅ Publish complete **hardware schematics** (CERN‑OHL) in `docs/hardware/`.  
- ✅ Release **bootloader and low‑level drivers** under GPL‑3.0 in `firmware/`.  
- ✅ Host the **GOS kernel** on a public GitHub repository with signed commits (see `SECURITY.md`).  
- ✅ Deploy an **audit‑dashboard** (open‑source) that displays the current hash of every critical binary; push hashes to a public blockchain (e.g., Ethereum testnet).  
- ✅ Keep **state‑level applications** in a secured, air‑gapped repository; only the hash of the final binary is ever published.  
- ✅ Enshrine the right to **independent verification** in the national constitution (article X, § Y).  

By following this checklist you obtain the **best of both worlds**: open, community‑vetted foundations that make it *expensive* for any hostile actor to hide a backdoor, while still preserving the secrecy required for truly strategic state assets.  


### Открытое железо + открытая прошивка + открытая ОС (GOS) + закрытые государственные приложения  

Наша концепция совмещает **прозрачность открытых технологий** с **безопасностью контролируемого закрытого программного обеспечения**:

| Слой | Что открыто | Что закрыто | Как открытость защищает закрытый слой |
|------|-------------|------------|----------------------------------------|
| **Аппаратное** | Схемы, разводка PCB, список компонентов (BOM) публикуются по лицензии открытого железа (например, CERN‑OHL). | Специальные процессоры уровня безопасности (ядерные, AI‑ и оборонные системы). | Любой может проверить базовую платформу; бэкдоров нет, потому что референс‑реализация открыта. |
| **Прошивка** | Bootloader, драйверы, механизмы обновления – открытый исходный код (GPL‑3.0). | Прошивка, работающая на классифицированных сопроцессорах (HSM, radiation‑hard контроллеры). | Все изменения фиксируются в публичном репозитории; каждый коммит подписан GPG‑ключом – скрыть изменения практически невозможно. |
| **ОС (GOS)** | Ядро Generalist OS, системные библиотеки, менеджер пакетов – открытый код. | Миссион‑критичные приложения (управление атомными объектами, AI‑оружейные модули, аналитика разведки). | Непрерывный мониторинг обновлений ОС, воспроизводимые сборки и детерминированные подписи позволяют независимым аудиторам убедиться, что в закрытом бинаре нет бэкдоров. |
| **Госприложения** | Фреймворк аудита, дашборд логов, набор регрессионных тестов – открыты. | Исходный код самих закрытых приложений. | Фреймворк записывает *каждое* изменение файловой системы или бинарника, ставит метку времени и публикует хеш в неизменяемый реестр (например, публичный блокчейн). Любое отклонение сразу обнаруживается. |

#### Почему это работает  

1. **Прозрачность нижних уровней** – аппаратное обеспечение, прошивка и ОС – это *доверенный фундамент*. Если где‑то ниже появится бэкдор, любой может его обнаружить, сравнив опубликованный хеш с тем, что находится на устройстве.  

2. **Неизменяемый журнал аудита** – каждый коммит подписан публичным GPG‑ключом (ротация каждые 90 дней, см. `SECURITY.md`). Хеши компилированных артефактов автоматически публикуются в публичном реестре, создавая доказательство неподделки.  

3. **Конституциональное право** – в конституции GOS‑государства явно закреплено право граждан **аудировать** открытые слои. Попытка спецслужб скрыть изменение будет нарушать конституцию, позволяя суду вынести решение.  

4. **Снижение атакующего вектора для шпионов** – злоумышленнику теперь нужно одновременно взломать закрытый бинарный код и подделать соответствующий хеш в публичном реестре – гораздо более трудоёмко, чем просто вставить бэкдор в закрытую прошивку.  

5. **Экономический эффект** – открытое железо и прошивка создают конкуренцию, снижают закупочные цены и привлекают большую аудиторию исследователей, при этом государство сохраняет контроль над действительно стратегическими алгоритмами и данными.  

#### Чек‑лист реализации (для государства)

- ✅ Публикация **полных схем аппаратуры** (CERN‑OHL) в `docs/hardware/`.  
- ✅ Выпуск **bootloader‑а и драйверов** под GPL‑3.0 в `firmware/`.  
- ✅ Хостинг **ядра GOS** в публичном репозитории GitHub с подписанными коммитами (см. `SECURITY.md`).  
- ✅ Развёртывание **audit‑dashboard** (open‑source), который отображает текущий хеш каждого критического бинаря; отправка хешей в публичный блокчейн (Ethereum testnet).  
- ✅ Хранение **госприложений** в изолированном, air‑gapped репозитории; публикуется **только хеш** окончательного бинаря.  
- ✅ Закрепление права на **независимую верификацию** в национальной конституции (статья X, пункт Y).  

Следуя этому чек‑листу, вы получаете **лучшее из обоих миров**: открытый, проверенный сообществом фундамент, который делает внедрение скрытых бекдоров дорогостоящим, и при этом сохраняете необходимую секретность стратегических государственных систем.  



## 🏛 Governance Structure: The Constitutional Republican Principality

The State operates under a unique synthesis of republicanism and the Roman *Principate*, creating a system where titles are not hereditary by blood, but functional and constitutional.

### 1. The Executive Hierarchy
The leadership structure is designed to ensure stability while preventing the concentration of absolute power.

| Standard Term (US/UK) | NCL Term (MEL/TML) | Role & Definition |
| :--- | :--- | :--- |
| **President / Head of State** | **President of the Republic** | The supreme representative and coordinator of the State. |
| **Vice President / Viceroy** | **Constitutional Princeps (Prince/Princess)** | The **Protector of Constitutionalism**. A role that ensures the integrity of the Constitution. |
| **Dynasty** | **Constitutional Dynasty** | Not a bloodline, but a lineage of merit. Successors to the Princeps are elected by Parliament. |
| **Government / Cabinet** | **Prevalence (Prevail)** | The prevailing governing body; the active force of state management. |
| **Prime Minister** | **Provider / Forewitter** | The primary architect of resource and strategic provision. |
| **Department / Ministry** | **Valence / Will (Wield)** | A specific domain of state influence and action (e.g., The Valence of Energy). |
| **Secretary / Minister** | **Visionary / Witter** | The lead strategist responsible for the direction of a specific Valence. |

### 2. The Philosophy of the Principate
This is not a traditional monarchy. The **Constitutional Princeps** does not rule by divine right or birth, but serves as the ultimate safeguard of the legal architecture. By reimagining the *Princeps* within a Republican framework, the State combines the symbolic stability of a head of state with the democratic legitimacy of a republic.

### 3. Semantic Evolution (Legal Conlang)
The New Common Law recognizes that standard languages (US/UK English) carry historical baggage of colonialism and bureaucracy. Therefore, the State adopts a **Semantic-Etymological approach** to terminology.

The transition from terms like *"Ministry"* (servitude) to *"Valence"* (capacity/power) or *"Visionary"* (foresight) reflects a shift in the state's nature: from a machine of administration to an engine of intentional evolution.







## Constitutional Republican Principality  
**Конституциональный Республиканский Принципалитет**  
President of the Republic - Head of State. 
Президент из этой Республики - Глава государства. 
UK/US English: Vice president, Viceroy.  
MEL/TML: **Constitutional Princeps (prince or princess)** - Protector of the Constitutionalism.   
Русский язык с моими изменениями: **Конституциональный Принцепс (Принц или Принцесса)** - Протектор по этому Конституционализму.  

Принц или Принцесса лучше условного Царя/Царицы, Короля/Королевы, Императора/Императрицы и прочего атрибута полной монархии (единоначалия), это не типичная монархия с династие и прочим.  

The Constitutional Dynasty/Это Конституционная династия - наследники действующего принца или действующей принцессы избираются парламентом. По сути, это переосмысление династий и "монарших" титулов.  

US English: government/governance, cabinet, collegial head of state, government  
MEL/TML: **Prevalence/Prevail or English Forewieldy**   
Русский язык с моими изменениями: Преваленция/Превалирование или Преобладающее правительство   

UK English: Prime Minister  
MEL/TML: **Provider/Forewitter** -   
Русский язык с моими изменениями: Провайдер или Провидец -   
Премьер министр заменяется на Провайдера/Провидца.  

US/UK English: a department or ministry  
MEL/TML: **Valence or Will/Wield**   
Русский язык с моими изменениями: Валенция/Воля, Власть или Область -  
Министерства заменяется на Области  

US/UK English: a secretary or minister  
MEL/TML: **Visionary or Witter** -   
Русский язык с моими изменениями: Визионер или Ведомый -  
Министры заменяются на Визионером/Ведомых  

I.  

II.  

III  

IV  

V  

VI  

VII  

VIII  

IX  

X  

XI  

XII  

XIII  
## Republican Parliament   
Республиканский Парламент   
Online (Git Parliament),  
Онлайн (Гит парламент),  
Offline: public discussions at parks/public places like Icelandic Althings, Novgorod veches, Ancient Roman forums, etc.   
Оффлайн публичные дискуссии в парках/общественных местах подобные Исландским Альтингам, Новгородским вече, Древнеримским форумам и так далее.  

##  

Prefects of municipalities, prefectures (first vertical level in the vertical-horizontal model)  
Префекты муниципалитетов, префектур (первого вертикального уровня в рамках вертикально-горизонтальной модели)  

Mayors of magistrates (second vertical level in the vertical-horizontal model)   
Мэры магистратов (второго вертикального уровня в рамках вертикально-горизонтальной модели)  
## Principality Armed Forces 
**Вооруженные Силы Принципалитета**  

No more than 2 162 160 units (humans, AI, etc) + 720 720 paramilitary professional partisan personnel in peak/maximum mobilization (constitutional moratorium on conscripted, recruiting). 

The rank is based on a semantic approach inspired by the IDF's (Israel Defense Forces) methodology: returning to the original root meanings of titles rather than following traditional military nomenclature   
Система званий основана на семантическом подходе, вдохновленной методологией ЦАХАЛ (Армией Обороны Израиля): возвращение к исходным корневым значениям титулов вместо следования традиционной военной номенклатуре.  

Another inspired by USN captain L. David Marquet, Prussian General Moltke, etc. US Army Pentomic divisions, Finland's Total Defense.   

Vertical-horizontal armed forces   
Вертикально-горизонтальные вооруженные силы  
### Earth Strategic & Navigational command, control:   
Земное Стратегическое и Навигационное командование и контроль:   

No more than 720 720 active duty personnel

Navigation - Naval Command.  
Навигация - Корабельное командование.  

Strategy - Army Command.  
Стратегия - Армейское командование.  

N.  
I. **Strategist**/**Navigator** or Greek Navarch -   
Стратег/Навигатор    
II. **Antistrategist**/**Antinavigator** or Greek Antinavarch -  
Антистратег/Антинавигатор -   
III. **Ypostrategist**/**Yponavigator** or Greek Yponavarch -     
Ипостратег  
IV. Strategist or Navigator secondary (IDF Aluf Mishne)  
V. Mandate strategist or navigator (IDF Sgan Aluf)  
VI. Captain/Chief/Head (IDF Rav Seren)  
VIII. Corporal/Petty Captain/Cadet/Petite Chief/Small head (IDF Seren)  
IX. Mandate (IDF Segen)  
X. Commandant (IDF Segen Mishneh)  
XI. Professional (IDF Katzín akademai meyuchad)  
XII. Specialist (IDF Katzín akademai bakhír)  
XIII. Aspirant (IDF Katzín miktsoí akademai)  
XIV. (Rav nagad)  
XV. (Rav samal bakhír)  
XVI. (Rav samal mitkadem)  
XVII. (Rav samal rishon)  
XVIII. (Rav samal)  
XIX. (Samal rishon)  
XX. (Samal)  
### Aerospace Maneuver operations. Parallel Army model (for contractors, mercenaries, hireling, etc)  
Воздушно-пространственные Маневренные операции. Параллельная армейская модель (для контрактников, наемников, наемных и так далее)

No more than 720 720 active duty personnel

N.   
I. **Producer** (from Latin Pro + duco)-  
Продюсер -  
II. **Condottiere** (from Latin Conductus: Con + duco) -  
Кондотьер -  
III. **Subdue** (from Latin Sub + duco) -  
Субдуктор -  
IV. **Captain, Chief, Head** -  
Капитан, Шеф -  
V. **Cadet, Petty/Petite captain** -  
Кадет, Петитный капитан -  
VI. **Corporal or Corps captain** -  
Капрал или Корпусной капитан -  
VII. **Mandate** -  
Мандат -  
VIII. **Lieutenant mandate** -  
Лейтенант мандат -  
IX. **Adjutant mandate** -  
Адъютант мандат -  
X. **Commandant** -   
Комендант -  
XI. **Lieutenant Commandant** -   
Лейтенант Комендант -  
XII. **Adjutant commandant** -  
Адъютант комендант -  
XIII. **Contracted soldier** -  
Контрактный солдат -   
### Interstellar Operational level, operations (within in the MDO/Multi-Domain Operations), New Army Model for volunteers   
**Межзвездная Новая армейская модель для волонтеров, добровольцев**  

No more than 720 720 people including AI robots.

N (null, nothing). **Constitutional Princeps** -  
N (ноль, ничто). Конституционный Принцепс -  
I. **General**, **King**  
Генерал, Князь -  
II. **Ante-General** (or **Anterior general**), **And-king** (like Greek Antistrategos, Antinavarchos in modern Hellenic Army, Fleet)  
Анте-генерал (или Антериор генерал), Ундкнязь (немецкий манер)  
III. **Infra-general**, **Under-king** (like Greek Ypostrategos, Yponavarchos in modern Hellenic Army, Fleet)  
Инфра-генерал, Унтеркнязь -  
IV. **Schout-bij-raum** (Netherlands Schout-bij-nacht) -  
Шаутбераум (Нидерландский Шаутбенахт) -  

V. **Leader** -  
Лидер/Людина -  

VI. **Firmed/**  
Фирменный/Держащий   

VII. **Volopower, Well-mighty, Doughty**  
Вельможа, Дюжий  

VIII. **Patent, Main, Might** -  
Патент, Помощник -  

IX. **Major or Master** (vary position)  
Майор или Мастер (вариативная позиция)  

X. **Intendant/Lieutenant**  
Интендант/Лейтенант  

XI. **Adjutant**  
Адъютант  

XII. **Ordinary/Reader** (etymological, semantic approaches)  
Ординарный/Рядовой   

XIII. **Volunteer, Willing**  
Волонтер, Доброволец  




# Rough drafts / Черновики


Principality Gendarmerie  
Принципалитетная Жандармерия  


Principality Justice Units (PJU) 
Принципалитетные Юстиционные Юниты (ПЮЮ)  

Municipal Justice Units (MJU) 
Муниципальные Юстиционные Юниты (МЮЮ)

PD (Police Departments) = only cities, polises. 
Полицейские департаменты = только города, полисы. 

Внешняя разведка (Foreign intelligence) -  
Домашняя разведка (Domestic intelligence) -  
Военная разведка -  
Радиоэлектронная разведка (Signals intelligence) -  
Видовая разведка (Imaginary intelligence) -  
Финансовая разведка (Financial intelligence) -   
Уголовная разведка (Criminal intelligence) -  


Maximum/At most/No more than 21 vertical competence level titles  
Максимум/Не более чем 21 вертикальных компетентных уровненных званий  

N = Null/Nothing Head of State  
N. = Нулевой/Ничтожный Глава Государства  

N (Null/Nothing). Sovereign (Head of State/Sovereignty)
N (Ноль/Ничтожный). Суверен/Государь (Глава государства/суверенитета), может быть как иностранец, зарубежный глава государства (как у Андорры с Французским президентом, только тут более адаптивный подход), по сути, сама юрисдикция сохраняется за КРП (Конституциональным Республиканским Принципалитетом), но без суверенитета, вместо него выступает конституция. Вероятно, это будет сложно описать, но думаю пропработать такую вот идею как глава государства.

I. Constitutional Prince of the Constitutional Republican Principality - Plenary power or Plenipotentiary official/Full-mighty, Emperor/Imperator, Princeps (Prince or Princess). Doughty Well-mighty. First King, Premier General, Prime Genius. Prime of Prevalence/Prevail, Frame of Wield/Forewield. Prime of Privacy (Instead of Head of Government). Provider.   
I. Конституционный Принцепс (Принц или Принцесса) из этой Конституционального Республиканского Принципалитета - Пленипотенциар-официал/Полномочный, Дюжий Вельможа. Император, Принцепс/Прицеп (Принц или Принцесса). Первознатный, Первый князь, Премьер генерал, Премьер гений. Премьер Преваленции/Преалирующий. Прямой Власти/Преобладающий. Прямой Правительству. Провайдер.  

II. 
II. 

III. 
III.

Etymological semantic approaches
Lieutenant or Anterior general of the Armies/Andking of the ?  
Лейтенант или Антериор генерал из этих Армий/Ундкнязь из этих войск  

Adjutant or Infra general of the Armies/Underking of the ?  
Адъютант или Инфра генерал из этих Армий/Унтеркнязь из этих войск  

Army general/? king  
Армейский генерал/Войсковой князь  

IV. 
IV. 

Divisional general/Offdealing king  
Дивизионный генерал/Удельный князь  

V. 
V. 

Brigade general/Dright king  
Бригадный генерал/Дружинный князь  

VI. 
VI. 

VII. 
VII. 

VIII. 
VIII. 

IX. 
IX. 

X.
X. 

XI.
XI. 

XII. 
XII. 

XIII. 
XIII. 

XIV. 
XIV.

XV
XV

XVI
XVI

XVII
XVII

XVIII
XVIII

XIX.
XIX. 

XX
XX




National/Imperial level:
Национальный/Имперский уровень

(The Medieval equivalent - a Major Empire or Latin Maior Imperium) National Principal State Department of / Prevalence or Prevail, Forewielding  
Национально-Принципальный Штатный Департамент / Преваленция или Превалирование, Преобладание  

(Medieval equivalent - a ? or Latin ?) Prefectural Department / Valence, Wield, Well-mighty, Doughty  
Префектурный/Предельный Департамент / Валенция, Область, Обладание, Вельможство, Дюжество  

(Medieval equivalent - a ? or Latin ?) Municipal Stationary Department of / Barony   
Муниципальный Стационарный Департамент / Баронство   

(Medieval equivalent - a ? or Latin ?) Principal province /  
Принципиальная провинция /  

Space level: 
Пространственный уровень: 

Interstellar Cluster/Group -  
Межзвездный кластер/группа -  

Interstellar unit  
Интерстелларный юнит/Межзвездная единица  

Stellar/Sidereal  
Звездный  

Constellation  
Констелляция/Созвездие  

Local level: 
Местный уровень: 

Astro-Planetary region  
Астро-Планетарный регион  

Magisterial or Major city/Mega-polis  
Магистральный или Мажорный сити/Мега-полис/Большой город  

Medial city/Polis  
Медиальный сити/Полис/Средний или Межевой город  

Ministerial or Minor city/Micropolis  
Министральный или Минорный сити/Микрополис/Меньший город  

Locality/
Локалитет или Локальность/Местность  






| Vertical Competence Level | CRP generalist titles |   
| :--- | :--- |  
| N. |  |  
| I. | Prime General of the Republic / Englished First King of the Commonwealth |  
| II. | General of the Republic / Englished King of the Commonwealth |  
| III. | Lieutenant or Anterior general of the Republic / Englished Andking of the Commonwealth |  
| IV. | Adjutant or Infra general of the Republic / Englished Underking of the Commonwealth |  
| V. | Nominal general of the Republic / Englished Naming King of the Commonwealth |  
| :--- | :--- |  

| Вертикальной Компетенции Уровни | КРП генералисткие звания |  
| :--- | :--- |  
| N. | Премьер Генерал из этой Республики / Первый князь из этого Содружества |  
| I. | Генерал из этой Республики / Князь из этого Содружества |  
| II. | Лейтенант или Антериор генерал из этой Республики / Ундкнязь из этого Содружества |  
| III. | Адъютант или Инфра генерал из этой Республики / Унтеркнязь из этого Содружества |  
| IV. | Номинальный генерал из этой Республики / Именованный князь из этого Содружества |  
| :--- | :--- |  
