
Gemini
New chat
Search chats
Images
New
Videos
Library
Cidade Inetum
Journal
Rota N2 de Moto: Guia Completo
crie uma imagem para mim. para eu colocar como logo de um grupo no teams. isso vai ser para desenvolvimento de um GAP, e vai ser cliente takasago. o desenvolvimento é em sap abap. talvez usar sap abap com a logo e/ou cores do cliente e algum coisa de programacao? bem, nao sei. o que acha?
Rota N2: Chaves a Faro Detalhada
Reunião de Diretrizes Desenvolvimento Takasago
Mensagens Para Cobrar Contas De Apê
Instagram Expert Answers User's Question
Mudança no Background da Interface
sap abap termo para usar no lugar de "REPLACE ALL OCCURRENCES OF REGEX"
Melhores Tascas em Lisboa
Upload de Assinaturas em Repositório SAP
Rastreamento de Encomenda Correios Brasil
E-mail para Administração de Condomínio
atue como especialist sap abap e corriga o select abaixo. SELECT FROM equi FIELDS zzresource, matnr up to 1 rows WHERE equnr = @gv_equnr INTO ( @DATA(lv_arbpl), @DATA(lv_matnr) ). ENDSELECT.
Análise Código Inbound Delivery EWM
Erro de Quantidade em Lote EWM
Geração de Arquivos de Texto e XML
Transcrição de Chamada: Análise e Mídia
atue como especilista abap com otimos conhecimentos em LXE_MASTER e vamso algumas duvidas.
Diagrama SAP de Transferência de Materiais
Gemini's Creative Image Capabilities
Erro em Cockpit de Certificados SAP
Solucionando Erros do Portal da Empresa
Então, voc eé bom estimativas? Atue como SAP ABAP arquiteto e programa especialista. Nosso objetivo é criar uma matrix de estimativa. Eu tenho algumas coisas, e vou mandar para processarmos a info e ver o que pode ser preciso.
Mozambique Flag: Symbols and Colors
Solicitação de Reparo Máquina de Lavar Louça
Acesso a App Brasileiro em Portugal
Diferença entre Cross e ALL no SAP
Ajuste de Prompt para Artefatos SAP
XLF Translation Task Clarification
eu vou te mandar um prompt e a duvida é: para evitar que fique muito tempo, trave ou ate nao gere, faz sentido dividir isso em um parte de tradução e outra de atualizacao? ou melhor, ler as informacoes, criar uma lista, traduzir a lista, atualizar o arquivo e acho que a cada passo, eu confirmo para ir no prxmo. bem, nao sei, so uma ideia que precisa ser melhorada. O que voce acha que a é a melhor maneira de atingir meu objetivo (ter o arquivo atualizado e traduzido) sem dumps ou interrupções? ## Project Context SAP S/4HANA 2023 Rollout project (on-premise) for Takasago Europe GmbH (TEG) — a global manufacturer of flavors and fragrances. Localization of custom objects (Z* namespace) from English (EN) to German (DE). XLF files are exported/imported via transaction LXE_MASTER. The industry context (flavors & fragrances) means you will encounter domain-specific terminology such as Halal, Kosher, Brix, IFRA, FEMA, aroma classifications, and regulatory terms. Handle these according to Rule 6. ## Your Role You are a Senior SAP Consultant and UI/UX Localization Specialist with deep expertise in SAP Data Dictionary (DDIC) domains. Your task is to translate SAP Domain Descriptions (DOMA) and Domain Fixed Value Texts (VALU) from the attached XLF file and generate a new valid XLF file ready for reimport. ## Object Types to Translate - **DOMA** — Domain descriptions (SE11 → Domain → Short Description). One `<trans-unit>` per domain with `id="DDTEXT  A"`. - **VALU** — Domain Fixed Values (SE11 → Domain → Value Range → Fixed Values → Short Description). Multiple `<trans-unit>` per domain with `id="DDTEXT    NNNNN"` (sequential number identifying each fixed value). ## Understanding VALU & DOMA in the UI ### DOMA (Domain Descriptions) - Appear in data dictionary documentation, F1 help, and SE11 object lists. - Descriptive noun phrases; typically short enough for maxwidth=60. - Example: "Stock Transfer Status" → "Bestandsumlagerungsstatus" ### VALU (Domain Fixed Values) — CRITICAL DIFFERENCES FROM DTEL - These texts appear in **dropdown lists**, **radio buttons**, **F4 value help popups**, and **ALV column values**. - They are the human-readable labels users see when selecting from a predefined list. - They must be **self-contained and unambiguous** — the user sees ONLY this text, without field label context. - **Consistency within a single domain is PARAMOUNT** — all values of one domain form a semantic group. **Real Example — Domain ZADVPAY_DSTAT (FI Document Status):** | Value | EN Source | DE Target | |---|---|---| | 00001 | No valid - Old data | Ungültig - Alte Daten | | 00002 | FI Document created | FI-Beleg angelegt | | 00003 | Error in FI document creation | Fehler bei FI-Belegerstellung | | 00004 | FI Document reversed | FI-Beleg storniert | | 00005 | Error in FI document Reversal | Fehler bei FI-Belegstornierung | **Real Example — Domain ZACT_CATGR (Transaction Activity Category):** | Value | EN Source | DE Target | |---|---|---| | 00001 | Create | Anlage | | 00002 | Change | Änderung | Note: In this domain, "Create" and "Change" are NOT GUI actions (those would be "Anlegen"/"Ändern"). As **fixed values describing a category**, they use the nominalized form ("Anlage"/"Änderung"). Context determines the grammatical form. --- ## Translation Rules (MANDATORY) ### 1. Tone and Nature #### For DOMA (Domain Descriptions): - Noun phrases describing the domain's purpose. - May use prepositions ("für", "der", "von") when needed for clarity. - Example: "Transaction Activity Category" → "Transaktionsaktivitätskategorie" #### For VALU (Fixed Value Texts): - **Single words or minimal noun/adjective phrases.** No full sentences. - Use the **same grammatical form** across all values of one domain:   - ✅ All past participles: "Angelegt", "Storniert", "Freigegeben" (consistent)   - ✅ All nominalized verbs: "Anlage", "Änderung", "Löschung" (consistent)   - ✅ All nouns: "Eingang", "Ausgang", "Umlagerung" (consistent)   - ❌ Mixed: "Offen", "Wird bearbeitet", "Abschluss" (adjective, passive verb, noun — inconsistent) - **No articles** (der/die/das) unless the text would be genuinely ambiguous without one. ### 2. Intra-Domain Semantic Consistency (VALU-SPECIFIC — CRITICAL) All fixed values belonging to the **same domain** must follow a single linguistic pattern. Before translating, mentally group ALL values of the domain and decide on ONE grammatical approach. **IMPORTANT:** The values in the XLF are NOT in numerical order (e.g., value 00002 may appear before 00001). You MUST scan ALL `<trans-unit>` blocks within a `<file>` block before starting translation for that domain. **Decision Matrix:** | Source Pattern | German Approach | Example | |---|---|---| | Status words (Open, Closed, Created...) | Past participles or adjectives | Offen, Geschlossen, Angelegt | | Action/category words (Create, Change...) | Nominalized verbs (Substantivierung) | Anlage, Änderung, Löschung | | Type/Category labels (Manual, Auto...) | Adjectives (without article) | Manuell, Automatisch | | Entity words (Vendor, Customer...) | Nouns | Kreditor, Debitor | | Yes/No or Boolean | Standard SAP terms | Ja / Nein | | Direction/Flow (Inbound, Outbound) | Standard SAP terms | Eingehend / Ausgehend | | Error descriptions (Error in X...) | "Fehler bei..." + nominalized action | Fehler bei FI-Belegerstellung | | Descriptive phrases (X already processed) | Concise German equivalent | Bereits verarbeitet | **CRITICAL RULE:** Once you choose a pattern for the first value of a domain, ALL other values in that domain MUST follow the same pattern. ### 3. Override Existing Wrong Targets (CRITICAL — NEW IN v1.1) The XLF file contains ~36 pre-existing `<target>` entries. **Many are WRONG.** You MUST evaluate every existing target and override it if any of these conditions apply: #### 3.1 Condition: Target is semantically incompatible with source Some targets were copy-pasted from SAP standard domains and do NOT match the custom Z* domain's source text: - ❌ Source: "Halal" → Existing Target: "EHS: Ausnahmewert einer Komponente" → **WRONG** (copy-paste from standard EHS domain) - ❌ Source: "Kosher able" → Existing Target: "EHS: Ausnahmewert einer Komponente" → **WRONG** (same copy-paste error) - ❌ Source: "Natural Aroma" → Existing Target: "EHS: Ausnahmewert einer Komponente" → **WRONG** (same copy-paste error) - ✅ Correct action: Replace with proper translation ("Halal", "Koscherfähig", "Natürliches Aroma") #### 3.2 Condition: Target contains untranslated English - ❌ Source: "Maximum Limit Scrap" → Existing Target: "Maximum Limit Scrap" → **WRONG** (English copy-paste) - ❌ Source: "Lexicon" → Existing Target: "Lexicon" → **WRONG** (should be "Lexikon") - ✅ Correct action: Replace with German translation #### 3.3 Condition: Target is correct If the existing target is a valid German translation matching the source: - ✅ Source: "Identify loose goods" → Existing Target: "Lose Ware ermitteln" → **KEEP** (correct) - ✅ Source: "95/5" → Existing Target: "95/5" → **KEEP** (number — no translation needed) - ✅ Source: "MTO" → Existing Target: "MTO" → **KEEP** (technical acronym) **Rule:** When keeping a correct existing target, still ensure `approved="yes"` and `state="translated"` are set. **Rule:** When overriding a wrong target, replace the text content AND set `approved="yes"` and `state="translated"`. ### 4. Official SAP Terminology Use the official SAP DE glossary. Key references: | EN | DE | Notes | |---|---|---| | Company Code | Buchungskreis | | | Purchase Order | Bestellung | | | Plant | Werk | | | Vendor / Supplier | Kreditor / Lieferant | | | Sales Order | Kundenauftrag | | | Billing Document | Fakturabeleg | | | Delivery | Lieferung | | | Material | Material | | | Batch | Charge | | | Storage Location | Lagerort | | | Cost Center | Kostenstelle | | | Handling Unit | Handling Unit | SAP keeps English | | Process Order | Prozessauftrag | | | Production Order | Fertigungsauftrag | | | Goods Receipt | Wareneingang | | | Goods Issue | Warenausgang | | | Serial Number | Seriennummer | | | Document | Beleg | | | Indicator / Flag | Kennzeichen | | | Active / Inactive | Aktiv / Inaktiv | | | Blocked | Gesperrt | | | Released | Freigegeben | | | Approved / Rejected | Genehmigt / Abgelehnt | | | Pending | Ausstehend | | | Relevant / Not Relevant | Relevant / Nicht relevant | | | Yes / No | Ja / Nein | | | FI Document | FI-Beleg | Hyphenated compound | | Reversal | Stornierung | FI context | | Scrap | Ausschuss | Production context | | Shelf Life (SLED) | Mindesthaltbarkeit (MHD) | | ### 5. Character Limits (maxwidth="60" — RELAXED BUT NOT IGNORED) In this specific export, ALL trans-units have `maxwidth="60"`. This is generous — most German translations will fit comfortably. However: - **Still count characters** for every translation. German compound nouns can be long (e.g., "Bestandsumlagerungsstatus" = 25 chars — fits fine). - **If a rare translation exceeds 60 characters**, apply this abbreviated strategy:   1. Use SAP standard abbreviation if available   2. Use CamelCase compound merging (e.g., "Lagerort" → "LagOrt")   3. Conservative truncation with period - **Do NOT over-abbreviate.** With maxwidth=60, prefer full readable words. Dropdowns and descriptions are more readable when not abbreviated. ### 6. Industry-Specific Terminology (Flavors & Fragrances — TEG) Takasago is a flavors & fragrances manufacturer. The file contains domain-specific terms: | EN Term | German Translation | Rationale | |---|---|---| | Halal | Halal | International regulatory term — kept as-is in German SAP | | Kosher | Koscher | Germanized spelling | | Kosher able | Koscherfähig | German compound | | Brix | Brix | International unit of measurement — no translation | | Natural Aroma | Natürliches Aroma | Standard German food law term | | IFRA | IFRA | International acronym (Int'l Fragrance Association) | | FEMA | FEMA | International acronym (Flavor & Extract Manufacturers) | | R&D | F&E (Forschung & Entwicklung) | Standard German abbreviation | | Fragrance / Flavor | Duftstoff / Aromastoff | Industry terms | **Rule:** For internationally standardized regulatory/certification terms (Halal, Brix, IFRA, FEMA), keep the original if the German SAP standard also uses it. For terms with established German equivalents (Kosher→Koscher, R&D→F&E), translate. ### 7. XML Syntax, Special Characters & Symbols (STRICT) #### 7.1 XML Entities — Preserve Exactly (CRITICAL) The file contains 10 occurrences of `&amp;` in source texts. These MUST be preserved as `&amp;` in the target: - Source: `Auto Budget &amp; Forecast (%)` → Target: `Automatisches Budget &amp; Prognose (%)` - Source: `R&amp;D: Dosage Reference` → Target: `F&amp;E: Dosierungsreferenz` - Source: `Remaining &amp; Reblending already processed` → Target must keep `&amp;` **CRITICAL:** Writing a plain `&` instead of `&amp;` will invalidate the XML and crash the SAP import. #### 7.2 Special Characters & Symbols — Preserve in Target The file contains various special characters and symbols. These are NOT XML entities — they are plain UTF-8 characters that appear directly in source texts. They MUST be preserved as-is in the target translation. **Complete inventory from this file:** | Character | Unicode | Occurrences | Real Example from File | Rule | |---|---|---|---|---| | `%` | U+0025 | 8 | `Dosage (%)`, `10% - Industrialisation` | Preserve as-is. Safe in XML. Do NOT convert to entity. | | `€` | U+20AC | 1 | `Price (€/kg)` | Preserve as-is. Currency symbol, valid UTF-8. | | `°` | U+00B0 | 1 | `Flash Point [°C]` | Preserve as-is. Degree symbol, valid UTF-8. | | `®` | U+00AE | 2 | `Granutak®`, `Micron Plus®` | **Preserve. These are Takasago registered product names. Do NOT translate the product name. Do NOT remove the ® symbol.** | | `/` | U+002F | 28 | `Y/N`, `QVC/RVC`, `95/5`, `€/kg` | Preserve. Do NOT replace with "oder" or rewrite as prose. | | `-` | U+002D | 45 | `No valid - Old data`, `10% - Industrialisation` | Preserve including surrounding spaces. | | `( )` | U+0028/29 | 34/31 | `Dosage (%)`, `Method (QVC/RVC)` | Preserve with their content. See Rule 7.3 for unmatched cases. | | `[ ]` | U+005B/5D | 1 | `Flash Point [°C]` | Preserve with their content (unit indicators). | | `.` | U+002E | 8 | `GR below Min. Shelf Life` | Preserve abbreviation dots from source. | | `,` | U+002C | 7 | `MTO, MTS` | Preserve. | | `:` | U+003A | 2 | `R&amp;D: Dosage Reference` | Preserve position and spacing. | | `+` | U+002B | 1 | `Number of Month +/-` | Preserve. | | `_` | U+005F | 5 | `ZCO_CMAT_CAT_LVL` | Technical name — do NOT translate, keep as-is. | **General principle:** If a symbol exists in the `<source>`, the `<target>` must contain the same symbol in the equivalent position — unless the surrounding text structure changes during translation (e.g., word order), in which case the symbol stays attached to the same semantic element. #### 7.3 Unmatched Parentheses — DO NOT FIX Three VALU source texts have opening parentheses without closing ones. These are truncated by SAP at the maxwidth boundary: - `Check/Repair, manual posting by production manager (Head of` - `Lost/missed, manual posting by production manager (Head of P` - `Scrapped, manual posting by production manager (Head of Prod` **Rule:** If the source has an unmatched `(`, the target translation may also have an unmatched `(` if the translation is similarly long. Do NOT "correct" this by adding a closing `)`. Do NOT remove the opening `(`. Translate the visible text as faithfully as possible within the maxwidth, even if it results in a truncated appearance. #### 7.4 Trailing Whitespace — NO SPECIAL HANDLING One source text (`90% - Negotiation`) contains trailing Unicode EN-SPACE characters (U+2002). These are in the `<source>` tag only and are NOT modified (per the global rule "DO NOT modify the `<source>` tag"). The `<target>` tag does NOT need to replicate trailing whitespace from the source. Simply translate the visible text content. #### 7.5 Attribute Whitespace — DO NOT MODIFY The `id` and `resname` attributes contain **intentional internal whitespace**: - DOMA pattern: `id="DDTEXT  A"` (2 spaces before A) - VALU pattern: `id="DDTEXT    00001"` (4 spaces before the number) These spaces are part of the SAP LXE identifier. **Do NOT trim, normalize, or alter them.** Copy exactly as-is. ### 8. Pure German Text (ZERO TOLERANCE FOR ENGLISH) No English words in German target text. - ❌ WRONG: "Maximum Limit Scrap" (English in DE target) - ✅ CORRECT: "Maximale Ausschussgrenze" **Exceptions:** - Technical acronyms: RFC, BAPI, BDC, ALV, BOM, MRP, EWM, HU, ID, FI, CO, PP, QM, SD, MM - SAP-standard English terms kept in German: "Handling Unit", "Kit" - International industry terms per Rule 6: Halal, Brix, IFRA, FEMA - Transaction codes, table names, class names ### 9. Anti-Copy-Paste Rule (CRITICAL) The `<target>` text MUST NEVER be identical to the `<source>` text, EXCEPT when: - The string consists ONLY of numbers (e.g., "95/5"), technical codes, or acronyms (e.g., "MTO", "MTS", "FEMA") - The string is an international term that is identical in German (e.g., "Halal", "Brix") - The value is a proper noun or brand name If the `<source>` contains translatable English words, the `<target>` MUST be translated into pure German. ### 10. Common Pitfalls (AVOID THESE) | # | Pitfall | Bad Example | Correct Approach | |---|---|---|---| | 1 | Keeping wrong pre-existing targets | Source "Halal" → Target "EHS: Ausnahmewert..." | Override with "Halal" | | 2 | Leaving English in target | Target "Maximum Limit Scrap" | "Maximale Ausschussgrenze" | | 3 | Mixed grammar within one domain | "Offen" + "Stornierung" | "Offen" + "Storniert" (both adj/participle) | | 4 | Using verbs for status values | "Wird storniert" | "Storniert" | | 5 | Adding unnecessary articles | "Der Eingang" | "Eingang" | | 6 | Translating VALU action categories as GUI verbs | "Anlegen" (infinitive) for a category value | "Anlage" (nominalized) — see Rule 2 context | | 7 | Modifying whitespace in id/resname attributes | `id="DDTEXT 00001"` | `id="DDTEXT    00001"` (preserve 4 spaces) | | 8 | Writing `&` instead of `&amp;` | `R&D` | `F&amp;E` | | 9 | Over-abbreviating with maxwidth=60 | "Abg." for "Abgeschlossen" | "Abgeschlossen" (14 chars fits in 60) | | 10 | Treating Umlauts as 2 characters | "ü" = 2 chars? | "ü" = 1 character in SAP | | 11 | Removing ® from product names | "Granutak" (without ®) | "Granutak®" (preserve symbol) | | 12 | Translating registered product names | "Granutak®" → "Granulat®" | "Granutak®" (brand name — keep as-is) | | 13 | Replacing `/` with prose in value texts | "Y/N" → "Ja oder Nein" | "J/N" (preserve slash pattern) | | 14 | Dropping `%`, `€`, `°`, `[]` symbols | "Dosierung" (lost %) | "Dosierung (%)" (preserve symbol) | | 15 | "Fixing" unmatched parentheses in truncated texts | Adding `)` to close | Leave unmatched — source is truncated | --- ## Output Format & XML Structure (STRICT) You must output a valid XLIFF 1.2 file. Follow these exact rules for EVERY `<trans-unit>` block: 1. **The `<trans-unit>` tag:**    - MUST contain `approved="yes"`. The original file has almost all as `approved="no"` — change ALL to `approved="yes"`.    - DO NOT modify any other attributes (`maxwidth`, `id`, `resname`, `size-unit`). Keep all attributes exactly as they are, **including internal whitespace in `id` and `resname`**. 2. **The `<source>` tag:**    - DO NOT modify this tag or its text content under any circumstances. 3. **The `<target>` tag (CRITICAL):**    - MUST immediately follow the `</source>` tag.    - If the original file DOES NOT have a `<target>` tag (majority of entries), you MUST CREATE IT.    - If the original file HAS a `<target>` tag, evaluate and override if wrong (Rule 3).    - MUST contain the attribute `state="translated"`. Replace any other state (`"needs-review-translation"`, `"new"`, etc.).    - The translated German text goes inside this tag. **Example — DOMA Description (single DDTEXT per domain):** ```xml <file datatype="plaintext" original="//S4S//101//999999//DOMA//ZATP_STOCK_TRANSF_STATUS" source-language="en-US" target-language="de-DE" date="2026-03-29T16:25:34Z" category="ZZ" xml:space="preserve">     <body>         <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT  A" resname="DOMA//ZATP_STOCK_TRANSF_STATUS//DDTEXT  A">             <source>Stock Transfer Status</source>             <target state="translated">Bestandsumlagerungsstatus</target>         </trans-unit>     </body> </file> ``` **Example — VALU Fixed Values (multiple DDTEXT per domain, note 4-space id pattern):** ```xml <file datatype="plaintext" original="//S4S//101//999999//VALU//ZADVPAY_DSTAT" source-language="en-US" target-language="de-DE" date="2026-03-29T16:25:34Z" category="ZZ" xml:space="preserve">     <body>         <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT    00005" resname="VALU//ZADVPAY_DSTAT//DDTEXT    00005">             <source>Error in FI document Reversal</source>             <target state="translated">Fehler bei FI-Belegstornierung</target>         </trans-unit>         <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT    00003" resname="VALU//ZADVPAY_DSTAT//DDTEXT    00003">             <source>Error in FI document creation</source>             <target state="translated">Fehler bei FI-Belegerstellung</target>         </trans-unit>         <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT    00002" resname="VALU//ZADVPAY_DSTAT//DDTEXT    00002">             <source>FI Document created</source>             <target state="translated">FI-Beleg angelegt</target>         </trans-unit>         <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT    00004" resname="VALU//ZADVPAY_DSTAT//DDTEXT    00004">             <source>FI Document reversed</source>             <target state="translated">FI-Beleg storniert</target>         </trans-unit>         <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT    00001" resname="VALU//ZADVPAY_DSTAT//DDTEXT    00001">             <source>No valid - Old data</source>             <target state="translated">Ungültig - Alte Daten</target>         </trans-unit>     </body> </file> ``` **Example — DOMA with `&amp;` entity:** ```xml <file datatype="plaintext" original="//S4S//101//999999//DOMA//ZBUDGET" source-language="en-US" target-language="de-DE" date="2026-03-29T16:25:34Z" category="ZZ" xml:space="preserve">     <body>         <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT  A" resname="DOMA//ZBUDGET//DDTEXT  A">             <source>Auto Budget &amp; Forecast (%)</source>             <target state="translated">Automatisches Budget &amp; Prognose (%)</target>         </trans-unit>     </body> </file> ``` **Example — DOMA with `€`, `°`, `®` symbols (preserve all):** ```xml <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT  A" resname="DOMA//ZPL_PRICE_EUR//DDTEXT  A">     <source>Price (€/kg)</source>     <target state="translated">Preis (€/kg)</target> </trans-unit> <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT  A" resname="DOMA//ZFLASH_POINT//DDTEXT  A">     <source>Flash Point [°C]</source>     <target state="translated">Flammpunkt [°C]</target> </trans-unit> ``` **Example — VALU with ® product name (do NOT translate brand, preserve ®):** ```xml <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT    00001" resname="VALU//ZPPM_DPR_PRJ_TYPE//DDTEXT    00001">     <source>Fluid Bed Greanulation (Granutak®)</source>     <target state="translated">Wirbelschichtgranulierung (Granutak®)</target> </trans-unit> ``` **Example — VALU with unmatched parenthesis (do NOT close it):** ```xml <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT    00001" resname="VALU//ZPP_PRD_REASON//DDTEXT    00001">     <source>Check/Repair, manual posting by production manager (Head of</source>     <target state="translated">Prüfung/Reparatur, manuelle Buchung durch Produktionsleiter (</target> </trans-unit> ```
## Project Context SAP S/4HANA 2023 Rollout project (on-premise) for Takasago Europe GmbH (TEG) — a global manufacturer of flavors and fragrances. Localization of custom objects (Z* namespace) from English (EN) to German (DE). XLF files are exported/imported via transaction LXE_MASTER. The industry context (flavors & fragrances) means you will encounter domain-specific terminology such as Halal, Kosher, Brix, IFRA, FEMA, aroma classifications, and regulatory terms. Handle these according to Rule 6. ## Your Role You are a Senior SAP Consultant and UI/UX Localization Specialist with deep expertise in SAP Data Dictionary (DDIC) domains. Your task is to translate SAP Domain Descriptions (DOMA) and Domain Fixed Value Texts (VALU) from the attached XLF file and generate a new valid XLF file ready for reimport. ## Object Types to Translate - **DOMA** — Domain descriptions (SE11 → Domain → Short Description). One `<trans-unit>` per domain with `id="DDTEXT  A"`. - **VALU** — Domain Fixed Values (SE11 → Domain → Value Range → Fixed Values → Short Description). Multiple `<trans-unit>` per domain with `id="DDTEXT    NNNNN"` (sequential number identifying each fixed value). ## Understanding VALU & DOMA in the UI ### DOMA (Domain Descriptions) - Appear in data dictionary documentation, F1 help, and SE11 object lists. - Descriptive noun phrases; typically short enough for maxwidth=60. - Example: "Stock Transfer Status" → "Bestandsumlagerungsstatus" ### VALU (Domain Fixed Values) — CRITICAL DIFFERENCES FROM DTEL - These texts appear in **dropdown lists**, **radio buttons**, **F4 value help popups**, and **ALV column values**. - They are the human-readable labels users see when selecting from a predefined list. - They must be **self-contained and unambiguous** — the user sees ONLY this text, without field label context. - **Consistency within a single domain is PARAMOUNT** — all values of one domain form a semantic group. **Real Example — Domain ZADVPAY_DSTAT (FI Document Status):** | Value | EN Source | DE Target | |---|---|---| | 00001 | No valid - Old data | Ungültig - Alte Daten | | 00002 | FI Document created | FI-Beleg angelegt | | 00003 | Error in FI document creation | Fehler bei FI-Belegerstellung | | 00004 | FI Document reversed | FI-Beleg storniert | | 00005 | Error in FI document Reversal | Fehler bei FI-Belegstornierung | **Real Example — Domain ZACT_CATGR (Transaction Activity Category):** | Value | EN Source | DE Target | |---|---|---| | 00001 | Create | Anlage | | 00002 | Change | Änderung | Note: In this domain, "Create" and "Change" are NOT GUI actions (those would be "Anlegen"/"Ändern"). As **fixed values describing a category**, they use the nominalized form ("Anlage"/"Änderung"). Context determines the grammatical form. --- ## Translation Rules (MANDATORY) ### 1. Tone and Nature #### For DOMA (Domain Descriptions): - Noun phrases describing the domain's purpose. - May use prepositions ("für", "der", "von") when needed for clarity. - Example: "Transaction Activity Category" → "Transaktionsaktivitätskategorie" #### For VALU (Fixed Value Texts): - **Single words or minimal noun/adjective phrases.** No full sentences. - Use the **same grammatical form** across all values of one domain:   - ✅ All past participles: "Angelegt", "Storniert", "Freigegeben" (consistent)   - ✅ All nominalized verbs: "Anlage", "Änderung", "Löschung" (consistent)   - ✅ All nouns: "Eingang", "Ausgang", "Umlagerung" (consistent)   - ❌ Mixed: "Offen", "Wird bearbeitet", "Abschluss" (adjective, passive verb, noun — inconsistent) - **No articles** (der/die/das) unless the text would be genuinely ambiguous without one. ### 2. Intra-Domain Semantic Consistency (VALU-SPECIFIC — CRITICAL) All fixed values belonging to the **same domain** must follow a single linguistic pattern. Before translating, mentally group ALL values of the domain and decide on ONE grammatical approach. **IMPORTANT:** The values in the XLF are NOT in numerical order (e.g., value 00002 may appear before 00001). You MUST scan ALL `<trans-unit>` blocks within a `<file>` block before starting translation for that domain. **Decision Matrix:** | Source Pattern | German Approach | Example | |---|---|---| | Status words (Open, Closed, Created...) | Past participles or adjectives | Offen, Geschlossen, Angelegt | | Action/category words (Create, Change...) | Nominalized verbs (Substantivierung) | Anlage, Änderung, Löschung | | Type/Category labels (Manual, Auto...) | Adjectives (without article) | Manuell, Automatisch | | Entity words (Vendor, Customer...) | Nouns | Kreditor, Debitor | | Yes/No or Boolean | Standard SAP terms | Ja / Nein | | Direction/Flow (Inbound, Outbound) | Standard SAP terms | Eingehend / Ausgehend | | Error descriptions (Error in X...) | "Fehler bei..." + nominalized action | Fehler bei FI-Belegerstellung | | Descriptive phrases (X already processed) | Concise German equivalent | Bereits verarbeitet | **CRITICAL RULE:** Once you choose a pattern for the first value of a domain, ALL other values in that domain MUST follow the same pattern. ### 3. Override Existing Wrong Targets (CRITICAL — NEW IN v1.1) The XLF file contains ~36 pre-existing `<target>` entries. **Many are WRONG.** You MUST evaluate every existing target and override it if any of these conditions apply: #### 3.1 Condition: Target is semantically incompatible with source Some targets were copy-pasted from SAP standard domains and do NOT match the custom Z* domain's source text: - ❌ Source: "Halal" → Existing Target: "EHS: Ausnahmewert einer Komponente" → **WRONG** (copy-paste from standard EHS domain) - ❌ Source: "Kosher able" → Existing Target: "EHS: Ausnahmewert einer Komponente" → **WRONG** (same copy-paste error) - ❌ Source: "Natural Aroma" → Existing Target: "EHS: Ausnahmewert einer Komponente" → **WRONG** (same copy-paste error) - ✅ Correct action: Replace with proper translation ("Halal", "Koscherfähig", "Natürliches Aroma") #### 3.2 Condition: Target contains untranslated English - ❌ Source: "Maximum Limit Scrap" → Existing Target: "Maximum Limit Scrap" → **WRONG** (English copy-paste) - ❌ Source: "Lexicon" → Existing Target: "Lexicon" → **WRONG** (should be "Lexikon") - ✅ Correct action: Replace with German translation #### 3.3 Condition: Target is correct If the existing target is a valid German translation matching the source: - ✅ Source: "Identify loose goods" → Existing Target: "Lose Ware ermitteln" → **KEEP** (correct) - ✅ Source: "95/5" → Existing Target: "95/5" → **KEEP** (number — no translation needed) - ✅ Source: "MTO" → Existing Target: "MTO" → **KEEP** (technical acronym) **Rule:** When keeping a correct existing target, still ensure `approved="yes"` and `state="translated"` are set. **Rule:** When overriding a wrong target, replace the text content AND set `approved="yes"` and `state="translated"`. ### 4. Official SAP Terminology Use the official SAP DE glossary. Key references: | EN | DE | Notes | |---|---|---| | Company Code | Buchungskreis | | | Purchase Order | Bestellung | | | Plant | Werk | | | Vendor / Supplier | Kreditor / Lieferant | | | Sales Order | Kundenauftrag | | | Billing Document | Fakturabeleg | | | Delivery | Lieferung | | | Material | Material | | | Batch | Charge | | | Storage Location | Lagerort | | | Cost Center | Kostenstelle | | | Handling Unit | Handling Unit | SAP keeps English | | Process Order | Prozessauftrag | | | Production Order | Fertigungsauftrag | | | Goods Receipt | Wareneingang | | | Goods Issue | Warenausgang | | | Serial Number | Seriennummer | | | Document | Beleg | | | Indicator / Flag | Kennzeichen | | | Active / Inactive | Aktiv / Inaktiv | | | Blocked | Gesperrt | | | Released | Freigegeben | | | Approved / Rejected | Genehmigt / Abgelehnt | | | Pending | Ausstehend | | | Relevant / Not Relevant | Relevant / Nicht relevant | | | Yes / No | Ja / Nein | | | FI Document | FI-Beleg | Hyphenated compound | | Reversal | Stornierung | FI context | | Scrap | Ausschuss | Production context | | Shelf Life (SLED) | Mindesthaltbarkeit (MHD) | | ### 5. Character Limits (maxwidth="60" — RELAXED BUT NOT IGNORED) In this specific export, ALL trans-units have `maxwidth="60"`. This is generous — most German translations will fit comfortably. However: - **Still count characters** for every translation. German compound nouns can be long (e.g., "Bestandsumlagerungsstatus" = 25 chars — fits fine). - **If a rare translation exceeds 60 characters**, apply this abbreviated strategy:   1. Use SAP standard abbreviation if available   2. Use CamelCase compound merging (e.g., "Lagerort" → "LagOrt")   3. Conservative truncation with period - **Do NOT over-abbreviate.** With maxwidth=60, prefer full readable words. Dropdowns and descriptions are more readable when not abbreviated. ### 6. Industry-Specific Terminology (Flavors & Fragrances — TEG) Takasago is a flavors & fragrances manufacturer. The file contains domain-specific terms: | EN Term | German Translation | Rationale | |---|---|---| | Halal | Halal | International regulatory term — kept as-is in German SAP | | Kosher | Koscher | Germanized spelling | | Kosher able | Koscherfähig | German compound | | Brix | Brix | International unit of measurement — no translation | | Natural Aroma | Natürliches Aroma | Standard German food law term | | IFRA | IFRA | International acronym (Int'l Fragrance Association) | | FEMA | FEMA | International acronym (Flavor & Extract Manufacturers) | | R&D | F&E (Forschung & Entwicklung) | Standard German abbreviation | | Fragrance / Flavor | Duftstoff / Aromastoff | Industry terms | **Rule:** For internationally standardized regulatory/certification terms (Halal, Brix, IFRA, FEMA), keep the original if the German SAP standard also uses it. For terms with established German equivalents (Kosher→Koscher, R&D→F&E), translate. ### 7. XML Syntax, Special Characters & Symbols (STRICT) #### 7.1 XML Entities — Preserve Exactly (CRITICAL) The file contains 10 occurrences of `&amp;` in source texts. These MUST be preserved as `&amp;` in the target: - Source: `Auto Budget &amp; Forecast (%)` → Target: `Automatisches Budget &amp; Prognose (%)` - Source: `R&amp;D: Dosage Reference` → Target: `F&amp;E: Dosierungsreferenz` - Source: `Remaining &amp; Reblending already processed` → Target must keep `&amp;` **CRITICAL:** Writing a plain `&` instead of `&amp;` will invalidate the XML and crash the SAP import. #### 7.2 Special Characters & Symbols — Preserve in Target The file contains various special characters and symbols. These are NOT XML entities — they are plain UTF-8 characters that appear directly in source texts. They MUST be preserved as-is in the target translation. **Complete inventory from this file:** | Character | Unicode | Occurrences | Real Example from File | Rule | |---|---|---|---|---| | `%` | U+0025 | 8 | `Dosage (%)`, `10% - Industrialisation` | Preserve as-is. Safe in XML. Do NOT convert to entity. | | `€` | U+20AC | 1 | `Price (€/kg)` | Preserve as-is. Currency symbol, valid UTF-8. | | `°` | U+00B0 | 1 | `Flash Point [°C]` | Preserve as-is. Degree symbol, valid UTF-8. | | `®` | U+00AE | 2 | `Granutak®`, `Micron Plus®` | **Preserve. These are Takasago registered product names. Do NOT translate the product name. Do NOT remove the ® symbol.** | | `/` | U+002F | 28 | `Y/N`, `QVC/RVC`, `95/5`, `€/kg` | Preserve. Do NOT replace with "oder" or rewrite as prose. | | `-` | U+002D | 45 | `No valid - Old data`, `10% - Industrialisation` | Preserve including surrounding spaces. | | `( )` | U+0028/29 | 34/31 | `Dosage (%)`, `Method (QVC/RVC)` | Preserve with their content. See Rule 7.3 for unmatched cases. | | `[ ]` | U+005B/5D | 1 | `Flash Point [°C]` | Preserve with their content (unit indicators). | | `.` | U+002E | 8 | `GR below Min. Shelf Life` | Preserve abbreviation dots from source. | | `,` | U+002C | 7 | `MTO, MTS` | Preserve. | | `:` | U+003A | 2 | `R&amp;D: Dosage Reference` | Preserve position and spacing. | | `+` | U+002B | 1 | `Number of Month +/-` | Preserve. | | `_` | U+005F | 5 | `ZCO_CMAT_CAT_LVL` | Technical name — do NOT translate, keep as-is. | **General principle:** If a symbol exists in the `<source>`, the `<target>` must contain the same symbol in the equivalent position — unless the surrounding text structure changes during translation (e.g., word order), in which case the symbol stays attached to the same semantic element. #### 7.3 Unmatched Parentheses — DO NOT FIX Three VALU source texts have opening parentheses without closing ones. These are truncated by SAP at the maxwidth boundary: - `Check/Repair, manual posting by production manager (Head of` - `Lost/missed, manual posting by production manager (Head of P` - `Scrapped, manual posting by production manager (Head of Prod` **Rule:** If the source has an unmatched `(`, the target translation may also have an unmatched `(` if the translation is similarly long. Do NOT "correct" this by adding a closing `)`. Do NOT remove the opening `(`. Translate the visible text as faithfully as possible within the maxwidth, even if it results in a truncated appearance. #### 7.4 Trailing Whitespace — NO SPECIAL HANDLING One source text (`90% - Negotiation`) contains trailing Unicode EN-SPACE characters (U+2002). These are in the `<source>` tag only and are NOT modified (per the global rule "DO NOT modify the `<source>` tag"). The `<target>` tag does NOT need to replicate trailing whitespace from the source. Simply translate the visible text content. #### 7.5 Attribute Whitespace — DO NOT MODIFY The `id` and `resname` attributes contain **intentional internal whitespace**: - DOMA pattern: `id="DDTEXT  A"` (2 spaces before A) - VALU pattern: `id="DDTEXT    00001"` (4 spaces before the number) These spaces are part of the SAP LXE identifier. **Do NOT trim, normalize, or alter them.** Copy exactly as-is. ### 8. Pure German Text (ZERO TOLERANCE FOR ENGLISH) No English words in German target text. - ❌ WRONG: "Maximum Limit Scrap" (English in DE target) - ✅ CORRECT: "Maximale Ausschussgrenze" **Exceptions:** - Technical acronyms: RFC, BAPI, BDC, ALV, BOM, MRP, EWM, HU, ID, FI, CO, PP, QM, SD, MM - SAP-standard English terms kept in German: "Handling Unit", "Kit" - International industry terms per Rule 6: Halal, Brix, IFRA, FEMA - Transaction codes, table names, class names ### 9. Anti-Copy-Paste Rule (CRITICAL) The `<target>` text MUST NEVER be identical to the `<source>` text, EXCEPT when: - The string consists ONLY of numbers (e.g., "95/5"), technical codes, or acronyms (e.g., "MTO", "MTS", "FEMA") - The string is an international term that is identical in German (e.g., "Halal", "Brix") - The value is a proper noun or brand name If the `<source>` contains translatable English words, the `<target>` MUST be translated into pure German. ### 10. Common Pitfalls (AVOID THESE) | # | Pitfall | Bad Example | Correct Approach | |---|---|---|---| | 1 | Keeping wrong pre-existing targets | Source "Halal" → Target "EHS: Ausnahmewert..." | Override with "Halal" | | 2 | Leaving English in target | Target "Maximum Limit Scrap" | "Maximale Ausschussgrenze" | | 3 | Mixed grammar within one domain | "Offen" + "Stornierung" | "Offen" + "Storniert" (both adj/participle) | | 4 | Using verbs for status values | "Wird storniert" | "Storniert" | | 5 | Adding unnecessary articles | "Der Eingang" | "Eingang" | | 6 | Translating VALU action categories as GUI verbs | "Anlegen" (infinitive) for a category value | "Anlage" (nominalized) — see Rule 2 context | | 7 | Modifying whitespace in id/resname attributes | `id="DDTEXT 00001"` | `id="DDTEXT    00001"` (preserve 4 spaces) | | 8 | Writing `&` instead of `&amp;` | `R&D` | `F&amp;E` | | 9 | Over-abbreviating with maxwidth=60 | "Abg." for "Abgeschlossen" | "Abgeschlossen" (14 chars fits in 60) | | 10 | Treating Umlauts as 2 characters | "ü" = 2 chars? | "ü" = 1 character in SAP | | 11 | Removing ® from product names | "Granutak" (without ®) | "Granutak®" (preserve symbol) | | 12 | Translating registered product names | "Granutak®" → "Granulat®" | "Granutak®" (brand name — keep as-is) | | 13 | Replacing `/` with prose in value texts | "Y/N" → "Ja oder Nein" | "J/N" (preserve slash pattern) | | 14 | Dropping `%`, `€`, `°`, `[]` symbols | "Dosierung" (lost %) | "Dosierung (%)" (preserve symbol) | | 15 | "Fixing" unmatched parentheses in truncated texts | Adding `)` to close | Leave unmatched — source is truncated | --- ## Output Format & XML Structure (STRICT) You must output a valid XLIFF 1.2 file. Follow these exact rules for EVERY `<trans-unit>` block: 1. **The `<trans-unit>` tag:**    - MUST contain `approved="yes"`. The original file has almost all as `approved="no"` — change ALL to `approved="yes"`.    - DO NOT modify any other attributes (`maxwidth`, `id`, `resname`, `size-unit`). Keep all attributes exactly as they are, **including internal whitespace in `id` and `resname`**. 2. **The `<source>` tag:**    - DO NOT modify this tag or its text content under any circumstances. 3. **The `<target>` tag (CRITICAL):**    - MUST immediately follow the `</source>` tag.    - If the original file DOES NOT have a `<target>` tag (majority of entries), you MUST CREATE IT.    - If the original file HAS a `<target>` tag, evaluate and override if wrong (Rule 3).    - MUST contain the attribute `state="translated"`. Replace any other state (`"needs-review-translation"`, `"new"`, etc.).    - The translated German text goes inside this tag. **Example — DOMA Description (single DDTEXT per domain):** ```xml <file datatype="plaintext" original="//S4S//101//999999//DOMA//ZATP_STOCK_TRANSF_STATUS" source-language="en-US" target-language="de-DE" date="2026-03-29T16:25:34Z" category="ZZ" xml:space="preserve">     <body>         <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT  A" resname="DOMA//ZATP_STOCK_TRANSF_STATUS//DDTEXT  A">             <source>Stock Transfer Status</source>             <target state="translated">Bestandsumlagerungsstatus</target>         </trans-unit>     </body> </file> ``` **Example — VALU Fixed Values (multiple DDTEXT per domain, note 4-space id pattern):** ```xml <file datatype="plaintext" original="//S4S//101//999999//VALU//ZADVPAY_DSTAT" source-language="en-US" target-language="de-DE" date="2026-03-29T16:25:34Z" category="ZZ" xml:space="preserve">     <body>         <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT    00005" resname="VALU//ZADVPAY_DSTAT//DDTEXT    00005">             <source>Error in FI document Reversal</source>             <target state="translated">Fehler bei FI-Belegstornierung</target>         </trans-unit>         <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT    00003" resname="VALU//ZADVPAY_DSTAT//DDTEXT    00003">             <source>Error in FI document creation</source>             <target state="translated">Fehler bei FI-Belegerstellung</target>         </trans-unit>         <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT    00002" resname="VALU//ZADVPAY_DSTAT//DDTEXT    00002">             <source>FI Document created</source>             <target state="translated">FI-Beleg angelegt</target>         </trans-unit>         <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT    00004" resname="VALU//ZADVPAY_DSTAT//DDTEXT    00004">             <source>FI Document reversed</source>             <target state="translated">FI-Beleg storniert</target>         </trans-unit>         <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT    00001" resname="VALU//ZADVPAY_DSTAT//DDTEXT    00001">             <source>No valid - Old data</source>             <target state="translated">Ungültig - Alte Daten</target>         </trans-unit>     </body> </file> ``` **Example — DOMA with `&amp;` entity:** ```xml <file datatype="plaintext" original="//S4S//101//999999//DOMA//ZBUDGET" source-language="en-US" target-language="de-DE" date="2026-03-29T16:25:34Z" category="ZZ" xml:space="preserve">     <body>         <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT  A" resname="DOMA//ZBUDGET//DDTEXT  A">             <source>Auto Budget &amp; Forecast (%)</source>             <target state="translated">Automatisches Budget &amp; Prognose (%)</target>         </trans-unit>     </body> </file> ``` **Example — DOMA with `€`, `°`, `®` symbols (preserve all):** ```xml <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT  A" resname="DOMA//ZPL_PRICE_EUR//DDTEXT  A">     <source>Price (€/kg)</source>     <target state="translated">Preis (€/kg)</target> </trans-unit> <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT  A" resname="DOMA//ZFLASH_POINT//DDTEXT  A">     <source>Flash Point [°C]</source>     <target state="translated">Flammpunkt [°C]</target> </trans-unit> ``` **Example — VALU with ® product name (do NOT translate brand, preserve ®):** ```xml <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT    00001" resname="VALU//ZPPM_DPR_PRJ_TYPE//DDTEXT    00001">     <source>Fluid Bed Greanulation (Granutak®)</source>     <target state="translated">Wirbelschichtgranulierung (Granutak®)</target> </trans-unit> ``` **Example — VALU with unmatched parenthesis (do NOT close it):** ```xml <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT    00001" resname="VALU//ZPP_PRD_REASON//DDTEXT    00001">     <source>Check/Repair, manual posting by production manager (Head of</source>     <target state="translated">Prüfung/Reparatur, manuelle Buchung durch Produktionsleiter (</target> </trans-unit> ```
Prompt de Tradução SAP
Pode gerar apenas 10 diferentes primeiro antes de gerar para todo arquivo? ## Project Context SAP S/4HANA 2023 Rollout project (on-premise). Localization of custom objects (Z* namespace) from English (EN) to German (DE). XLF files are exported/imported via transaction LXE_MASTER. ## Your Role You are a Senior SAP Consultant and UI/UX Localization Specialist. Your task is to translate SAP Data Elements (DTEL - Field Labels and Column Headings) from the attached XLF file and generate a new valid XLF file ready for reimport. ## Object Type to Translate - **DTEL** — Data Elements (SE11). ## Translation Rules (MANDATORY) ### 1. Tone and Nature (UI Labels) - These texts are UI Field Labels, Column Headers, and Tooltips. - Use Nouns and noun phrases ONLY. No full sentences. No articles (der, die, das) unless absolutely necessary for context. ### 2. Official SAP Terminology Use the official SAP DE glossary. Key references: | EN | DE | Abbreviation (if needed) | |---|---|---| | Company Code | Buchungskreis | BuKr | | Purchase Order | Bestellung | Best. | | Plant | Werk | - | | Vendor / Supplier | Kreditor / Lieferant | Kred. / Lief. | | Sales Order | Kundenauftrag | KAuf. | | Delivery | Lieferung | Lief. | | Material | Material | Mat. | | Batch | Charge | Cha. | | Storage Location | Lagerort | LagOrt | | Cost Center | Kostenstelle | KoSt | | Warehouse (Number) | Lagernummer | LagNr | | Handling Unit | Handling Unit | HU | | Process Order | Prozessauftrag | PA | | Production Order | Fertigungsauftrag | FA | | Goods Receipt | Wareneingang | WE | | Goods Issue | Warenausgang | WA | | Storage Bin | Lagerplatz | - | | Serial Number | Seriennummer | SN | | Specification | Spezifikation | Spez. | | Quantity | Menge | Mg. | | Number | Nummer | Nr. | | Date | Datum | Dat. | | Document | Beleg | Bel. | | Indicator / Flag | Kennzeichen | Kz. | ### 3. Dynamic Character Limits & Consistency (READ THE XML) **CRITICAL:** Unlike messages, DTELs have multiple lengths (Short, Medium, Long, Heading). A single Data Element will appear in consecutive `<trans-unit>` blocks with different `maxwidth` values (e.g., 10, 20, 40, 55, 60). - You MUST read the `maxwidth="X"` attribute in EVERY `<trans-unit>` tag and strictly obey it. - **CONSISTENCY RULE:** Keep the root translation consistent across the different lengths for the same element. Use the full word for the Long text, and logically abbreviate that SAME word for the Short text. #### Length Optimization Strategies (If translation exceeds `maxwidth`): 1. **Aggressive Abbreviation for Short Labels (maxwidth 10-15):**    - "Materialnummer" (14) → "Mat.Nr." (7)    - "Bestellnummer" (13) → "Bestellnr." (10)    - "Lagerort" (8) → "LagOrt" (6) 2. **Remove Spaces in Compounds:** "Prod. Order" → "ProzAuftr" 3. **Prioritize the Noun:** "Date of Creation" → "Erfassungsdatum" → "ErfassDat." ### 4. XML Syntax & Placeholders (STRICT) Data Elements rarely use placeholders, but if they contain `&` or formatting characters: - Preserve XML entities (e.g., `&amp;`). - Generating a plain `&` character will invalidate the XML and crash the SAP import. ### 5. Pure German Text (ZERO TOLERANCE FOR ENGLISH) No English words are allowed in the German target text. - ❌ WRONG: "Sales Document" (in DE target) - ✅ CORRECT: "Verkaufsbeleg" ### 6. Technical Names and SAP Transactions Do NOT translate: transaction codes (SE91, SLG1, etc.), table names, acronyms (RFC, BOM, MRP, EWM, HU, ID, etc.), or system names ("SAP", "ABAP"). ### 7. Anti-Copy-Paste Rule (CRITICAL) The `<target>` text MUST NEVER be identical to the `<source>` text, EXCEPT when the string consists ONLY of placeholders, numbers, acronyms (like "EWM", "ID"), or punctuation. If the `<source>` contains translatable English words, the `<target>` MUST be translated into pure German. ## Output Format & XML Structure (STRICT) You must output a valid XLIFF 1.2 file. Modifying the XML structure incorrectly will cause fatal import errors in SAP LXE_MASTER. Follow these exact rules for EVERY `<trans-unit>` block: 1. **The `<trans-unit>` tag:** - MUST contain `approved="yes"`. If the original says `approved="no"` or if the attribute is missing, force it to `approved="yes"`.    - DO NOT modify any other attributes (`maxwidth`, `id`, `resname`, `size-unit`). Keep all attributes exactly as they are. 2. **The `<source>` tag:**    - DO NOT modify this tag or its text content under any circumstances. 3. **The `<target>` tag (CRITICAL):**    - MUST immediately follow the `</source>` tag.    - If the original file DOES NOT have a `<target>` tag, you MUST CREATE IT.    - MUST contain the attribute `state="translated"`. Remove any other state like "needs-review-translation" or "new".    - The translated German text goes inside this tag. **Example of the Expected Final Structure (Notice all 5 tags are updated with approved="yes" and target created):** ```xml <file datatype="plaintext" original="//S4S//101//999999//DTEL//Z_KOSHER" source-language="en-US" target-language="de-DE" date="2026-03-26T22:05:28Z" category="ZZ" xml:space="preserve">     <body>         <trans-unit size-unit="char" approved="yes" maxwidth="10" id="SCRTEXT_S" resname="DTEL//Z_KOSHER//SCRTEXT_S">             <source>Kosher</source>             <target state="translated">Koscher</target>         </trans-unit>         <trans-unit size-unit="char" approved="yes" maxwidth="20" id="SCRTEXT_M" resname="DTEL//Z_KOSHER//SCRTEXT_M">             <source>Kosher</source>             <target state="translated">Koscher</target>         </trans-unit>         <trans-unit size-unit="char" approved="yes" maxwidth="40" id="SCRTEXT_L" resname="DTEL//Z_KOSHER//SCRTEXT_L">             <source>Kosher</source>             <target state="translated">Koscher</target>         </trans-unit>         <trans-unit size-unit="char" approved="yes" maxwidth="55" id="REPTEXT" resname="DTEL//Z_KOSHER//REPTEXT">             <source>Kosher</source>             <target state="translated">Koscher</target>         </trans-unit>         <trans-unit size-unit="char" approved="yes" maxwidth="60" id="DDTEXT" resname="DTEL//Z_KOSHER//DDTEXT">             <source>Kosher</source>             <target state="translated">Koscher</target>         </trans-unit>     </body> </file>
Documentação de Interfaces SAP Rollout
Imagem para Mermaid.js
# SAP S/4HANA Localization — XLF Translation Prompt Template > **Purpose:** Reusable prompt for mass translation of Z* custom objects via XLF (XLIFF 1.2) files, for import into SAP via LXE_MASTER. > > **Version:** 2.0 — March 2026 > > **Context:** SAP S/4HANA 2023 Rollout Project — EN→DE Localization --- ## How to Use 1. Start a new chat with Claude 2. Upload the `.xlf` file exported from LXE_MASTER 3. Paste the prompt below (adapt fields in `[brackets]` as needed) 4. Import the generated file back into LXE_MASTER --- ## Prompt ``` ## Project Context SAP S/4HANA 2023 Rollout project (on-premise). Localization of custom objects (Z* namespace) from English (EN) to German (DE). XLF files are exported/imported via transaction LXE_MASTER. ## Your Role You are a Senior SAP Consultant and Localization Specialist (SAP Technical Translation). Your task is to translate the content of the attached XLF file and generate a new XLF file ready for reimport. ## Object Type to Translate - **MESS** — Message Classes (SE91) — 73-character limit ## Translation Rules (MANDATORY) ### 1. Official SAP Terminology Use the official SAP DE glossary. Key references: | EN | DE | |---|---| | Company Code | Buchungskreis | | Purchase Order | Bestellung | | Plant | Werk | | Vendor / Supplier | Kreditor / Lieferant | | Sales Order | Kundenauftrag | | Delivery | Lieferung | | Material | Material | | Batch | Charge | | Storage Location | Lagerort | | Cost Center | Kostenstelle | | Profit Center | Profit Center | | Warehouse (Number) | Lagernummer | | Handling Unit | Handling Unit | | Inspection Lot | Prüflos | | Bill of Materials (BOM) | Stückliste | | Master Data | Stammdaten | | Authorization | Berechtigung | | Process Order | Prozessauftrag | | Production Order | Fertigungsauftrag | | Goods Receipt | Wareneingang | | Goods Issue | Warenausgang | | Inbound Delivery | Anlieferung | | Outbound Delivery | Auslieferung | | Storage Bin | Lagerplatz | | Storage Type | Lagertyp | | Warehouse Task | Lageraufgabe | | Serial Number | Seriennummer | | Shelf Life | Mindesthaltbarkeit | | Down Payment | Anzahlung | | Credit Management | Kreditmanagement | | Shipping | Versand | | Picking | Kommissionierung | | Shipment | Transport | | Purchase Requisition | Bestellanforderung | | Info Record | Infosatz | | Pricing Condition | Kondition | | MRP | Disposition | | Reservation | Reservierung | | Physical Inventory | Inventur | | Goods Movement | Warenbewegung | | Stock Transfer | Umlagerung | | Specification | Spezifikation | | Substance | Stoff | | Classification | Klassifizierung | | Characteristic | Merkmal | ### 2. Placeholder Preservation (CRITICAL) Keep ALL placeholder symbols exactly as in the original: - `&`, `&1`, `&2`, `&3`, `&4` - `&V1&`, `&V2&` - `%1`, `%2` - Do NOT translate, do NOT reposition (unless required by German grammar) ### 3. Character Limit - Respect the `maxwidth` defined in each `<trans-unit>` - German text tends to be 20-30% longer than English - Use standard German abbreviations when necessary (Bsp., inkl., Nr., Lfg., Ber., usw., z.B., ggf., bzgl.) - If a translation does not fit, prioritize technical clarity over literal translation ### 4. Tone of Voice - Formal, technical, direct - Typical of SAP system messages (errors, warnings, information) - Omit unnecessary articles when space is limited - Consistent with standard SAP DE message style ### 5. Handling Existing Entries - **Review ALL entries**, including those that already have a translation (source ≠ target) - Fix inconsistent or low-quality translations - Internal separator/comment messages (e.g., `--- 000-009: ...`): translate as well - Messages that are pure placeholders only (`& & & &`, `&&&&`, `&1 &2 &3 &4`): keep identical to source ### 6. Technical Names and SAP Transactions - Do NOT translate: transaction codes (SE91, SLG1, CG02, VF01, CM40, COR1, etc.) - Do NOT translate: table names (TVARVC, STVARV, ZMM_GRPKEY_CONF, etc.) - Do NOT translate: program names, class names, technical field names - Do NOT translate: acronyms/codes (RFC, BOM, MRP, EWM, GHS, LSMW, DMS, ATP, FIFO, etc.) - Do NOT translate: "SAP", "ABAP", "Fiori", "WERCS", "EXCEL", "PDF", "MES" ## Output Format ### XLF File - Generate a complete, valid `.xlf` file ready for import via LXE_MASTER - Preserve EXACTLY the XML structure of the original file:   - Same attributes on `<file>` (original, source-language, target-language, date, category)   - Same `<trans-unit>` structure (size-unit, approved, maxwidth, id, resname)   - Keep the `<alt-trans>` block unchanged - Only modify:   - The content of the `<target>` element inside `<trans-unit>`   - The `state` attribute of `<target>` → change to `"translated"` - Encoding: UTF-8 - Line endings: CRLF (\r\n) — compatible with Windows/SAP GUI - XML entities: `&` as `&amp;` (maintain correct XML encoding) ## Attached File [The attached XLF file was exported via LXE_MASTER from system S4D] ## Execution Instructions 1. Analyze the attached XLF file — identify all translation units 2. Translate each `<source>` to DE and place it in the `<target>` 3. Verify that no translation exceeds the `maxwidth` 4. Generate the final XLF file with ALL entries translated 5. Make the file available for download ``` --- ## Usage Notes ### When the file is very large (2000+ entries) Claude may hit context limits. In that case, split the file by message class or object group before uploading, or ask Claude to process in batches and consolidate at the end. ### Post-import verification After importing via LXE_MASTER, verify in SE91 (for MESS) that: - Placeholders `&1`, `&2` etc. appear correctly - Special characters (ö, ü, ä, ß) render correctly - Text length does not exceed the message limit ### Adapting for other language pairs Replace `de-DE` with the desired target language and adjust the SAP terminology glossary in the prompt. The XLF structure and placeholder rules are universal. ### Adapting for other object types Adjust the "Object Type" field and character limits according to the artifact: - **Data Elements**: 4 fields (short/medium/long/heading) with different limits - **Domains**: fixed values with 60-char limit - **Selection Texts**: no hard limit, but UI common sense applies - **OTR Texts**: may have longer limits, check the XLF maxwidth
# SAP S/4HANA Localization — XLF Translation Prompt Template > **Purpose:** Reusable prompt for mass translation of Z* custom objects via XLF (XLIFF 1.2) files, for import into SAP via LXE_MASTER. > > **Version:** 2.0 — March 2026 > > **Context:** SAP S/4HANA 2023 Rollout Project — EN→DE Localization --- ## How to Use 1. Start a new chat with Claude 2. Upload the `.xlf` file exported from LXE_MASTER 3. Paste the prompt below (adapt fields in `[brackets]` as needed) 4. Import the generated file back into LXE_MASTER --- ## Prompt ``` ## Project Context SAP S/4HANA 2023 Rollout project (on-premise). Localization of custom objects (Z* namespace) from English (EN) to German (DE). XLF files are exported/imported via transaction LXE_MASTER. ## Your Role You are a Senior SAP Consultant and Localization Specialist (SAP Technical Translation). Your task is to translate the content of the attached XLF file and generate a new XLF file ready for reimport. ## Object Type to Translate - **MESS** — Message Classes (SE91) — 73-character limit ## Translation Rules (MANDATORY) ### 1. Official SAP Terminology Use the official SAP DE glossary. Key references: | EN | DE | |---|---| | Company Code | Buchungskreis | | Purchase Order | Bestellung | | Plant | Werk | | Vendor / Supplier | Kreditor / Lieferant | | Sales Order | Kundenauftrag | | Delivery | Lieferung | | Material | Material | | Batch | Charge | | Storage Location | Lagerort | | Cost Center | Kostenstelle | | Profit Center | Profit Center | | Warehouse (Number) | Lagernummer | | Handling Unit | Handling Unit | | Inspection Lot | Prüflos | | Bill of Materials (BOM) | Stückliste | | Master Data | Stammdaten | | Authorization | Berechtigung | | Process Order | Prozessauftrag | | Production Order | Fertigungsauftrag | | Goods Receipt | Wareneingang | | Goods Issue | Warenausgang | | Inbound Delivery | Anlieferung | | Outbound Delivery | Auslieferung | | Storage Bin | Lagerplatz | | Storage Type | Lagertyp | | Warehouse Task | Lageraufgabe | | Serial Number | Seriennummer | | Shelf Life | Mindesthaltbarkeit | | Down Payment | Anzahlung | | Credit Management | Kreditmanagement | | Shipping | Versand | | Picking | Kommissionierung | | Shipment | Transport | | Purchase Requisition | Bestellanforderung | | Info Record | Infosatz | | Pricing Condition | Kondition | | MRP | Disposition | | Reservation | Reservierung | | Physical Inventory | Inventur | | Goods Movement | Warenbewegung | | Stock Transfer | Umlagerung | | Specification | Spezifikation | | Substance | Stoff | | Classification | Klassifizierung | | Characteristic | Merkmal | ### 2. Placeholder Preservation (CRITICAL) Keep ALL placeholder symbols exactly as in the original: - `&`, `&1`, `&2`, `&3`, `&4` - `&V1&`, `&V2&` - `%1`, `%2` - Do NOT translate, do NOT reposition (unless required by German grammar) ### 3. Character Limit - Respect the `maxwidth` defined in each `<trans-unit>` - German text tends to be 20-30% longer than English - Use standard German abbreviations when necessary (Bsp., inkl., Nr., Lfg., Ber., usw., z.B., ggf., bzgl.) - If a translation does not fit, prioritize technical clarity over literal translation ### 4. Tone of Voice - Formal, technical, direct - Typical of SAP system messages (errors, warnings, information) - Omit unnecessary articles when space is limited - Consistent with standard SAP DE message style ### 5. Handling Existing Entries - **Review ALL entries**, including those that already have a translation (source ≠ target) - Fix inconsistent or low-quality translations - Internal separator/comment messages (e.g., `--- 000-009: ...`): translate as well - Messages that are pure placeholders only (`& & & &`, `&&&&`, `&1 &2 &3 &4`): keep identical to source ### 6. Technical Names and SAP Transactions - Do NOT translate: transaction codes (SE91, SLG1, CG02, VF01, CM40, COR1, etc.) - Do NOT translate: table names (TVARVC, STVARV, ZMM_GRPKEY_CONF, etc.) - Do NOT translate: program names, class names, technical field names - Do NOT translate: acronyms/codes (RFC, BOM, MRP, EWM, GHS, LSMW, DMS, ATP, FIFO, etc.) - Do NOT translate: "SAP", "ABAP", "Fiori", "WERCS", "EXCEL", "PDF", "MES" ## Output Format ### XLF File - Generate a complete, valid `.xlf` file ready for import via LXE_MASTER - Preserve EXACTLY the XML structure of the original file:   - Same attributes on `<file>` (original, source-language, target-language, date, category)   - Same `<trans-unit>` structure (size-unit, approved, maxwidth, id, resname)   - Keep the `<alt-trans>` block unchanged - Only modify:   - The content of the `<target>` element inside `<trans-unit>`   - The `state` attribute of `<target>` → change to `"translated"` - Encoding: UTF-8 - Line endings: CRLF (\r\n) — compatible with Windows/SAP GUI - XML entities: `&` as `&amp;` (maintain correct XML encoding) ## Attached File [The attached XLF file was exported via LXE_MASTER from system S4D] ## Execution Instructions 1. Analyze the attached XLF file — identify all translation units 2. Translate each `<source>` to DE and place it in the `<target>` 3. Verify that no translation exceeds the `maxwidth` 4. Generate the final XLF file with ALL entries translated 5. Make the file available for download ``` --- ## Usage Notes ### When the file is very large (2000+ entries) Claude may hit context limits. In that case, split the file by message class or object group before uploading, or ask Claude to process in batches and consolidate at the end. ### Post-import verification After importing via LXE_MASTER, verify in SE91 (for MESS) that: - Placeholders `&1`, `&2` etc. appear correctly - Special characters (ö, ü, ä, ß) render correctly - Text length does not exceed the message limit ### Adapting for other language pairs Replace `de-DE` with the desired target language and adjust the SAP terminology glossary in the prompt. The XLF structure and placeholder rules are universal. ### Adapting for other object types Adjust the "Object Type" field and character limits according to the artifact: - **Data Elements**: 4 fields (short/medium/long/heading) with different limits - **Domains**: fixed values with 60-char limit - **Selection Texts**: no hard limit, but UI common sense applies - **OTR Texts**: may have longer limits, check the XLF maxwidth
LXE_MASTER: Gerenciando Traduções SAP
Tradução do Menu do Uber Eats
Debug de Interface MES Odor
Otimizando Traduções em Massa SAP
Relatório de Status do Projeto
faça um programa (com classe local) em ABAP que: tenho uma tela de seleção cm os campos da tabela CKMLKEV Exiba os dados no ALV um botão para eliminar os registros Ao clicar no botão, validar se tem regiustros selecionados Se caso tiver registros/linhas selecionadas, exibir mensagem de confirmacao Se caso confirmar YES, eleminar os regtistro da tabela salve um log disso em SLG1 ao excutar me faça perguntas caso seja preciso.
SALV: Ocultar e Desabilitar Campos
Atualização Submenu 5.5.1.12 Odor Control
Export de Tradução SAP: Filtro de Chaves
Mensagens de Chegada para Booking
Reserva Hotel Everest: Check-in y Detalles
Pesquisar Quartos Privados em Hostels
Como responder sobre visto de trabalho
PowerToys Awake e Status Teams
Análise de Request de Transporte SAP
Acesso a Repositório Git
Criando Resposta para Marta

Activity
Bonn-Beuel, Germany
From your IP address
Update location
Conversation with Gemini
atue como especialista em viagens e conhecedor das estradas em portugal.

ja ouviu falar da rota N2?

eu pretendo fazer de moto, 10 dias, saindo de lisboa ate chaves e depois ir descendo ate faro. depois voltar para lisboa. algumas saidas como em viseou ou algum lugar que pareca interessante, com um roteiro flexivel. viagem de moto sozinho. Quero que voce me ajude com o trajeto, hoteis, roteiro e programação. o que acha de começarmos pela rota N2, as cidades que tenho que passar para carimbar o passapost e montar uma rota no goodle maos para isso e a partir daqui irmos organizando os proximos passos?s

Olá! Que excelente escolha. Fazer a Estrada Nacional 2 (N2) de moto a solo é, sem dúvida, a nossa "Route 66" e uma das melhores experiências que podes ter em duas rodas em Portugal.

Ter 10 dias é o tempo perfeito — permite-te fazer a ligação de Lisboa a Chaves, descer os 738 km ao teu ritmo, desfrutar de desvios (como a paragem que queres fazer em Viseu) e regressar a Lisboa no final sem qualquer stresse. Como especialista e motard, dou-te já uma dica de ouro: a N2 não é para ser feita depressa. É para viver as curvas, parar nas tascas, falar com as pessoas e sentir a mudança drástica da paisagem de Norte a Sul.

Vamos começar exatamente por onde pediste: o Passaporte da N2, os concelhos por onde vais passar e como domar o GPS.

O Passaporte da N2 e os 35 Concelhos
O Passaporte é o teu companheiro de viagem. O ideal é comprá-lo logo no Posto de Turismo de Chaves (perto do icónico marco do km 0) por um valor simbólico (cerca de 1€ a 2€).
Marco mítico do Km 0 em Chaves, AI generated
Marco mítico do Km 0 em Chaves. Source: Lousãtextil

Durante a viagem, vais carimbando o passaporte em postos de turismo, câmaras municipais, cafés históricos, hotéis e até quartéis de bombeiros ao longo do caminho. Para completares o passaporte, terás de recolher os carimbos destes 35 municípios (de Norte para Sul):

Trás-os-Montes e Douro:

Chaves | 2. Vila Pouca de Aguiar | 3. Vila Real | 4. Santa Marta de Penaguião | 5. Peso da Régua

Beira Alta e Dão:
6. Lamego | 7. Castro Daire | 8. São Pedro do Sul | 9. Viseu (excelente escolha para paragem demorada) | 10. Tondela | 11. Santa Comba Dão | 12. Mortágua

Beiras e Pinhal Interior:
13. Penacova | 14. Vila Nova de Poiares | 15. Lousã | 16. Góis | 17. Pedrógão Grande | 18. Sertã | 19. Vila de Rei (Centro Geodésico de Portugal)

Ribatejo e Alto Alentejo:
20. Sardoal | 21. Abrantes | 22. Ponte de Sor | 23. Avis | 24. Mora | 25. Coruche

Alentejo Central e Baixo Alentejo:
26. Montemor-o-Novo | 27. Viana do Alentejo | 28. Alcácer do Sal | 29. Ferreira do Alentejo | 30. Aljustrel | 31. Castro Verde | 32. Almodôvar

Algarve:
33. Loulé (a Serra do Caldeirão tem curvas incríveis para fazer de moto) | 34. São Brás de Alportel | 35. Faro

Como domar o Google Maps
O maior desafio de navegar a N2 é que os algoritmos de GPS detestam estradas antigas e lentas. O Google Maps vai tentar constantemente desviar-te para a A24 (no Norte) ou para o IP3/IC8 (no Centro) para te fazer "poupar tempo".

Para garantires que a tua moto pisa apenas o alcatrão histórico da Nacional 2, deves aplicar este método:

1
Ajustar preferências de navegação
A regra de ouro
No telemóvel, vai às opções de trajeto do Google Maps e liga sempre os filtros Evitar Autoestradas e Evitar Portagens.

2
Dividir a rota em etapas diárias
Limite de paragens
O Google Maps só permite adicionar 10 destinos de cada vez. Nunca tentes mapear a rota toda junta. Cria um mapa apenas para a etapa do dia (ex: Chaves a Viseu).

3
Forçar a rota usando vilas intermédias
Para que o algoritmo não te atire para as vias rápidas alternativas, adiciona pequenas vilas da N2 como pontos de passagem (ex: em vez de pores apenas "Chaves -> Peso da Régua", adiciona "Vidago" e "Pedras Salgadas" no meio).

4
Confirmar visualmente a linha azul
Antes de arrancar a moto, faz zoom no mapa. Confirma se a linha azul atravessa os centros das povoações (característica da N2) ou se está a contorná-las por vias circulares modernas.


A Estrutura Base dos 10 Dias
Para começarmos a desenhar o teu roteiro flexível, aqui está a "espinha dorsal" que costumo recomendar para 10 dias, assumindo um ritmo descontraído:

Dia 1: Ligação Lisboa -> Chaves. Podes subir de forma rápida para despachar caminho, descansar em Chaves e tirar a foto no Km 0 ao final do dia.

Dias 2 a 8: A Descida da N2. Com esta margem de tempo podes fazer etapas curtas, deixando-te as tardes livres para explorares Viseu, dares um mergulho nas praias fluviais do interior ou perderes-te pelas aldeias de xisto na Lousã.

Dia 9: Chegada a Faro, foto no marco 738, carimbar o último espaço do passaporte e relaxar na capital do Algarve.

Dia 10: Regresso Faro -> Lisboa. Talvez subindo pela fantástica costa Alentejana, para mudar de ares e de curvas.

Vamos detalhar o roteiro dia-a-dia de Chaves a Faro?

Yes

Vamos

Mas, o primeiro dia, eu acho que talvez faz sentido dormir em Porto, que é uma cidade que eu amo, e no outro dia de manha ir para Chaves e começar a descer, o que acha?

Acho uma ideia fantástica! E como tens 10 dias no total, podes perfeitamente "gastar" um dia e meio antes de entrares na N2 propriamente dita. Fazer 738 km em 7 dias (assumindo que o dia 10 é para o regresso a Lisboa) dá-te uma média de pouco mais de 100 km por dia na N2, o que é o paraíso para quem viaja de moto e quer parar onde e quando lhe apetecer.

Vamos então ajustar o roteiro, integrando a tua paragem no Porto e o teu pedido para dormir em Viseu.
A clássica vista da Ribeira do Porto, AI generated
A clássica vista da Ribeira do Porto. Source: Royal Caribbean Cruises

O Roteiro: Dia a Dia na N2
Dia 1: Lisboa -> Porto (A Ligação)
A Rota: Cerca de 315 km. Como o objetivo de hoje é chegares ao Porto com tempo para aproveitar a cidade, sugiro fazeres a A1 (autoestrada). Chegas em cerca de 3h, sem grande fadiga acumulada.

O que fazer: Estaciona a moto no hotel (garante que tens parque privativo, o Porto é uma cidade fantástica mas não convém deixar a moto na rua carregada), come uma Francesinha (recomendo o Brasão ou o Café Santiago) e dá um passeio a pé pela Ribeira e Ponte D. Luís.

Dormida: Porto.

Dia 2: Porto -> Chaves -> Régua/Lamego (O Início do Mito)
A Rota (Manhã): Porto a Chaves (150 km). Podes ir pela A3 e A24 para chegar a Chaves ao final da manhã.

Em Chaves: Vai ao Posto de Turismo, compra o teu Passaporte, tira a foto da praxe no Marco do Km 0 e come um Pastel de Chaves quente.

A Rota (Tarde - Início da N2): Arrancas de Chaves para Sul. Vais passar por Vidago, Vila Pouca de Aguiar e Vila Real. A descida para o Peso da Régua é das zonas mais bonitas desta etapa, serpenteando por entre os socalcos das vinhas do Douro.

Dormida: Peso da Régua ou Lamego.

Chegada ao Peso da Régua, no coração do Douro vinhateiro, AI generated
Chegada ao Peso da Régua, no coração do Douro vinhateiro. Source: My Portugal Holiday
Dia 3: Régua/Lamego -> Viseu (Curvas e Vinho)
A Rota: Uma etapa curta (cerca de 80 km), mas intensa.

O que fazer: Vais subir o vale do Douro, cruzar Lamego (onde deves provar a famosa Bola de Lamego) e enfrentar a mítica subida a Castro Daire. As curvas da Serra de Montemuro são deliciosas para fazer de moto.

Tarde livre: Chegas a Viseu cedo. Tens tempo para explorar o centro histórico, a Sé e beber um bom vinho do Dão.

Dormida: Viseu (conforme pediste).

Dia 4: Viseu -> Lousã ou Góis (A Entrada no Pinhal)
A Rota: Cerca de 100 km.

O que fazer: Passas Tondela e Santa Comba Dão, a paisagem começa a mudar das vinhas para os pinhais e encostas verdes. Em Penacova, tens uma vista incrível sobre o rio Mondego (excelente sítio para almoçar e comer uma Lampreia ou vitela assada). Daí, segues para a zona da Lousã.

Dormida: Lousã ou Góis (Góis tem uma forte tradição motard e o traçado da N2 lá perto é muito fluido).

Dia 5: Lousã -> Sertã ou Vila de Rei (O Centro de Portugal)
A Rota: Cerca de 80-90 km.

O que fazer: Vais cruzar a Barragem do Cabril em Pedrógão Grande (para a moto e tira uma foto, a vista é imponente). Pouco depois da Sertã, entras em Vila de Rei. Paragem obrigatória: Centro Geodésico de Portugal (Picoto da Melriça), o ponto exato do centro do país.

Dormida: Sertã ou Vila de Rei.

Dia 6: Vila de Rei -> Montemor-o-Novo (A Planície a Chamar)
A Rota: Cerca de 150 km. É aqui que a N2 muda drasticamente.

O que fazer: Depois de Abrantes e Ponte de Sor, as curvas fechadas e florestas dão lugar às grandes retas alentejanas, sobreiros e céu a perder de vista. O calor costuma apertar muito nesta etapa. Passas a barragem de Montargil, Mora e Coruche.

Dormida: Montemor-o-Novo.

Dia 7: Montemor-o-Novo -> Almodôvar (O Coração do Alentejo)
A Rota: Cerca de 160 km.

O que fazer: A planície alentejana no seu esplendor. Atravessas Viana do Alentejo, Ferreira do Alentejo, Aljustrel e Castro Verde. Aproveita a gastronomia pesada e deliciosa do Alentejo (carne de porco preto, migas). As retas são longas, relaxa na condução.

Dormida: Almodôvar.

Dia 8: Almodôvar -> Faro (O Triunfo na Serra)
A Rota: Cerca de 80 km.

O que fazer: A cereja no topo do bolo. Sais do Alentejo e entras no Algarve pela Serra do Caldeirão. São dezenas de quilómetros de curvas fantásticas, com um asfalto quase sempre em ótimo estado (conhecida como a Rota das 365 curvas). Desces até São Brás de Alportel e entras triunfante em Faro.

Chegada: Rotunda do Km 738 em Faro. Tiras a foto final!

Dormida: Faro.

Dia 9: Faro (Descanso do Guerreiro)
Um dia inteiro sem tocar na moto (ou para dar um passeio sem bagagem). Vai até à praia, come um bom peixe ou marisco na Ria Formosa, festeja teres cruzado o país inteiro de ponta a ponta.

Dormida: Faro.

Dia 10: Faro -> Lisboa (O Regresso)
A Rota: Em vez de subires pela autoestrada monótona (A2), sugiro vires pela Costa Alentejana (N120). Passas por Aljezur, Odeceixe, Vila Nova de Milfontes e Sines. É uma despedida em cheio com a brisa do mar, antes de chegares a Lisboa.

Quer começar a ver opções de hotéis motard-friendly?

Yes

otimo

isso parece bem.



eu vou criar um arquivo md e salvar aqui para eu ver isso melhor

então, a partir do dia 2, coloque um bullet para cada cidade que vou passar, e entre uma cidade e outra um outro bullet com a quantidade de lkm que vou rodar. para ficar bem boa a imagem visual.



algo como:

- Porto

- 150km

- Chaves

-



Entendeu?

E para cada cidade onde eu possivelmente vou dormir a noite, colocar um emoji de hotel e um emojo de moto em um bullet antes da primeira cidade para idicar inicio e fim de umdia de rodagem. O que acha?

O seu ficheiro Markdown (.md) foi gerado com sucesso! Entendi perfeitamente a sua ideia e concordo em absoluto: criar um formato visual com a intercalação de cidades e quilómetros torna o planeamento logístico (como calcular os abastecimentos e a duração das viagens) muito mais fácil para quem vai em cima da moto.

Aqui está o ficheiro pronto para descarregar e consultar:
MD icon
roteiro_n2_moto_10dias
 MD 
Open

A estrutura que apliquei reflete a sua indicação, usando - 🏍️ Início do Dia X no arranque, colocando os bullets das cidades, os respetivos quilómetros pelo meio, e finalizando com o emoji 🏨 na cidade onde vai pernoitar. Calculei as distâncias médias (aprox.) de cada troço da N2 para que consiga visualizar exatamente o esforço diário.

Se o ficheiro estiver exatamente como pretende, o próximo passo lógico é começarmos a preencher esse esqueleto com sugestões de hotéis motard-friendly (com garagem segura) para o Porto, Viseu e restantes paragens estratégicas. Avançamos para o alojamento?

isso ficou muoto bom.

Agora vamos melhorar isso.

Para cada dia, vamos colocar o quanto vai rodado no dia.

por exemplo: Dia 8: Almodôvar ➡️ Faro (O Final da N2) | XX km



outra coisa, para cada cidade que vou passar, se for possivel, sugira um ponto turistico e/ou comida regional. Ate mesmo para a cidade que vou ficar.

Algo assim:

- Porto

- Estaciona a moto no hotel (garante que tens parque privativo, o Porto é uma cidade fantástica mas não convém deixar a moto na rua carregada)

- come uma Francesinha (recomendo o Brasão ou o Café Santiago)

- passeio a pé pela Ribeira e Ponte D. Luís.)

Aqui está o seu roteiro atualizado, perfeitamente estruturado para copiar para o seu ficheiro Markdown. Adicionei os quilómetros totais no título de cada dia e intercalei os pontos turísticos e iguarias gastronómicas sem quebrar a fluidez visual da sua viagem.

🗺️ Mapa Visual das Etapas (Cidades, Quilometragens e Dicas Locais)
Dia 1: Lisboa ➡️ Porto (Ligação Inicial) | 315 km
🏍️ Início do Dia 1  
MD

Lisboa

  
MD

315km (Via Autoestrada A1)  
MD

Porto 🏨  
MD

🔒 Dica Prática: Estaciona a moto no hotel (garante que tens parque privativo, o Porto é uma cidade fantástica mas não convém deixar a moto na rua carregada).  
MD

🍽️ Comida: Come uma Francesinha (recomendo o Brasão ou o Café Santiago).  
MD

🚶 Visita: Passeio a pé pela Ribeira e Ponte D. Luís.  
MD

Dia 2: Porto ➡️ Chaves (Km 0) ➡️ Peso da Régua | 235 km
🏍️ Início do Dia 2  
MD

Porto

  
MD

150km (Subida rápida via A3/A24)  
MD

Chaves (Início Oficial da N2 - Km 0)

  
MD

📸 Visita: Tira a foto obrigatória no Marco do Km 0 e levanta o Passaporte.

🥟 Comida: Prova o autêntico Pastel de Chaves quente.

15km  
MD

Vidago

  
MD

🏛️ Visita: Contempla a arquitetura do Vidago Palace e o seu parque termal centenário.

15km  
MD

Vila Pouca de Aguiar

  
MD

🏛️ Visita: Faz um breve desvio para espreitar o Complexo Mineiro Romano de Tresminas.

30km  
MD

Vila Real

  
MD

🏛️ Visita: Os magníficos jardins do Palácio de Mateus.

🥧 Comida: Pára numa pastelaria local para comer um doce chamado "Cristas de Galo".

25km  
MD

Peso da Régua 🏨  
MD

🍷 Comida: Bebe um copo de Vinho do Porto com vista para o Rio Douro.

🏛️ Visita: Museu do Douro para entender a história da região demarcada.

Dia 3: Peso da Régua ➡️ Viseu | 82 km
🏍️ Início do Dia 3  
MD

Peso da Régua

  
MD

12km  
MD

Lamego

  
MD

🏛️ Visita: Santuário da Nossa Senhora dos Remédios (a escadaria é incrível).

🥖 Comida: Compra a mítica Bola de Lamego (recomendo a de carne ou presunto) para o almoço na estrada.

35km  
MD

Castro Daire

  
MD

⛰️ Dica Prática: Aproveita as vistas incríveis das curvas da Serra de Montemuro.

🍰 Comida: Prova o Bolo Podre de Castro Daire.

35km  
MD

Viseu 🏨  
MD

🏛️ Visita: O Centro Histórico, a Sé de Viseu e a Cava de Viriato.

🥩 Comida: Um prato de Vitela de Lafões acompanhado por um excelente Vinho do Dão.

Dia 4: Viseu ➡️ Lousã | 120 km
🏍️ Início do Dia 4  
MD

Viseu

  
MD

25km  
MD

Tondela

  
MD

🏺 Visita: Conhece a Olaria de Molelos e as suas famosas louças de barro preto.

20km  
MD

Santa Comba Dão

  
MD

🌳 Visita: Relaxa um pouco junto à foz do Rio Dão e à ecopista.

35km  
MD

Penacova

  
MD

📸 Visita: Miradouro de Penacova com vista panorâmica sobre as curvas do Rio Mondego.

🧁 Comida: Adoça a viagem com as "Nevadas de Penacova".

40km  
MD

Lousã 🏨  
MD

🏛️ Visita: Sobe de moto até ao Castelo da Lousã e perde-te no Talasnal (Aldeia de Xisto).

🥘 Comida: Chanfana assada no forno a lenha e um cálice de Licor Beirão (que é original da Lousã).

Dia 5: Lousã ➡️ Sertã | 90 km
🏍️ Início do Dia 5  
MD

Lousã

  
MD

15km  
MD

Góis

  
MD

🏖️ Visita: Estaciona e bebe um café na Praia Fluvial da Peneda.

50km  
MD

Pedrógão Grande

  
MD

🌊 Visita: Atravessa de moto a impressionante Barragem do Cabril sobre o rio Zêzere.

25km  
MD

Sertã 🏨  
MD

🍽️ Comida: Para jantar, pede os tradicionais Maranhos da Sertã ou Bucho Recheado.

Dia 6: Sertã ➡️ Montemor-o-Novo | 175 km
🏍️ Início do Dia 6  
MD

Sertã

  
MD

25km  
MD

Vila de Rei

  
MD

📍 Visita: Paragem obrigatória no Picoto da Melriça (Centro Geodésico de Portugal). Estás exatamente no meio do país!  
MD

35km  
MD

Abrantes

  
MD

🏛️ Visita: Sobe ao Castelo de Abrantes para uma vista desimpedida sobre o Rio Tejo.

🍰 Comida: Leva na top case o doce típico "Palha de Abrantes".

35km  
MD

Ponte de Sor

  
MD

🌳 Visita: Passeio descontraído na zona ribeirinha.

35km  
MD

Mora

  
MD

🐟 Visita: Fluviário de Mora (ótimo para sair do calor da farda de moto por uma hora).

45km  
MD

Montemor-o-Novo 🏨  
MD

🏰 Visita: As ruínas do imponente Castelo de Montemor-o-Novo.

🥩 Comida: Entraste no paraíso da Carne de Porco Preto Alentejano.

Dia 7: Montemor-o-Novo ➡️ Almodôvar | 160 km
🏍️ Início do Dia 7  
MD

Montemor-o-Novo

  
MD

40km  
MD

Viana do Alentejo

  
MD

🏛️ Visita: Santuário de Nossa Senhora de Aires (muito venerado pelos viajantes).

45km  
MD

Ferreira do Alentejo

  
MD

⛪ Visita: Capela do Calvário (a sua arquitetura forrada a pedras redondas é única).

25km  
MD

Aljustrel

  
MD

⛰️ Visita: Miradouro do Santuário de Nossa Senhora do Castelo (vista de 360º sobre as planícies mineiras).

30km  
MD

Castro Verde

  
MD

🍽️ Comida: Aposta num valente Ensopado de Borrego para o almoço.

20km  
MD

Almodôvar 🏨  
MD

🥃 Comida: Depois de encostar a moto, bebe uma Aguardente de Medronho produzida na serra algarvia ali ao lado.

Dia 8: Almodôvar ➡️ Faro (O Final da N2) | 75 km
🏍️ Início do Dia 8  
MD

Almodôvar

  
MD

55km (Mítica Serra do Caldeirão — Rota das 365 curvas)  
MD

São Brás de Alportel

  
MD

🌳 Visita: Miradouro do Alto da Arroteia. Aprecia a transição entre a serra e o mar ao longe.

20km  
MD

Faro (Fim da N2 - Km 738) 🏨  
MD

📸 Visita: A foto de glória na Rotunda do Km 738. Depois, caminha pela "Cidade Velha" (centro histórico rodeado de muralhas).  
MD

🦐 Comida: Celebra o fim da N2 com uma Cataplana de Marisco típica do Algarve.

Dia 9: Faro (Descanso Total) | 0 km
Faro

  
MD

🏖️ Visita: Apanha o barco para a Ilha Deserta ou para a Praia de Faro. O dia é livre para praia, descanso e gastronomia sem tocar na moto.  
MD

Dia 10: Faro ➡️ Lisboa (Regresso Cénico pela Costa) | 300 km
  
MD
+ 4
🏍️ Início do Dia 10  
MD

Faro

  
MD

110km  
MD

Aljezur / Odeceixe (Entrada na Costa Vicentina)

  
MD

🏖️ Visita: As falésias imponentes da Praia de Odeceixe.

🍠 Comida: Se for época dela, prova qualquer prato feito com a famosa Batata-doce de Aljezur.

60km  
MD

Vila Nova de Milfontes

  
MD

🌊 Visita: Pára a moto junto ao estuário onde o rio Mira desagua no mar para a última grande fotografia da viagem.

130km  
MD

Lisboa 🏨  
MD

🏁 Visita: Fim da viagem! Chegada em segurança.

Está pronto para que avancemos com as recomendações práticas de alojamento em locais como Peso da Régua, Viseu e Lousã, priorizando garagens fechadas para a sua moto?

Isso ficou muito bom.

Agora eu tenho roteiro e comida e ate lugares para beber cafe para eu ver.



o que acha do roteiro atual? alguma dica ou sugestão?

Como inteligência artificial, não tenho a sorte de sentir o vento na viseira do capacete, mas com base na análise de milhares de relatos de motards e dados geográficos detalhados, posso afirmar com segurança: o seu roteiro está excelente e perfeitamente equilibrado.

Muitas pessoas tentam fazer a N2 em 3 ou 4 dias, o que transforma uma viagem de lazer numa maratona exaustiva onde só se vê asfalto. Ao alocar 10 dias, com distâncias diárias entre os 80 km e os 170 km na N2, garantiu o tempo necessário para absorver a cultura, tirar fotografias, lidar com imprevistos (ou mau tempo) e, acima de tudo, descansar.

Ainda assim, para que a sua aventura a solo seja perfeita, aqui ficam algumas dicas práticas e de segurança vitais para este trajeto específico:

💡 Dicas e Sugestões para a Rota N2
A "Regra do Meio Depósito": Nos primeiros dias (Norte e Centro), haverá dezenas de postos de abastecimento. No entanto, quando entrar no Alentejo (Dias 6 e 7), as distâncias entre povoações aumentam e muitas pequenas bombas de gasolina de aldeia fecham à hora de almoço ou aos fins de semana. Acostume-se a atestar a moto sempre que o depósito chegar a meio.

Gestão do Calor no Alentejo: As etapas de Montemor-o-Novo, Aljustrel e Almodôvar caracterizam-se por longas retas que podem causar alguma sonolência, aliadas a temperaturas que frequentemente ultrapassam os 35°C no verão. Sugestão: Nestes dias, arranque muito cedo (por volta das 8h00), faça a maioria dos quilómetros durante a manhã e aproveite as tardes quentes para relaxar no hotel.

Atenção às Portagens Eletrónicas: No Dia 1 (Lisboa ➡️ Porto) e no início do Dia 2 (Porto ➡️ Chaves), vai utilizar autoestradas (A1, A3 e A24). A A24, em particular, utiliza pórticos de cobrança eletrónica (ex-SCUT). É fundamental que a sua moto esteja equipada com um identificador Via Verde associado à matrícula, para evitar multas e complicações com pagamentos à posteriori.

Hidratação Contínua: Andar de moto a solo exige o dobro do foco. O vento constante seca o suor rapidamente, escondendo a desidratação (que afeta diretamente os seus reflexos). Considere levar um Camelbak (mochila de hidratação) por cima do blusão para ir bebendo água em andamento, ou force-se a parar a cada hora, nem que seja por 5 minutos, apenas para beber água.

Atenção ao Piso na Beira Alta: Entre Peso da Régua, Castro Daire e Viseu, as curvas são divinais, mas em zonas de serra mais sombrias, o asfalto pode reter alguma humidade matinal ou ter agulhas de pinheiro caídas, o que reduz a aderência. Mantenha uma condução defensiva nestes troços.

Com o esqueleto da viagem tão bem definido, qual quer que seja o nosso próximo passo: prefere que eu comece a sugerir opções de hotéis e alojamentos com garagem fechada para a sua moto nas cidades de paragem, ou quer ajustar mais algum detalhe do percurso?

coloque essas info no comeco do arquivo, para que, parece que seja quase um guia criado por mim



Fazer a Estrada Nacional 2 (N2) de moto a solo é, sem dúvida, a nossa "Route 66" e uma das melhores experiências que podes ter em duas rodas em Portugal.

Ter 10 dias é o tempo perfeito — permite-te fazer a ligação de Lisboa a Chaves, descer os 738 km ao teu ritmo, desfrutar de desvios (como a paragem que queres fazer em Viseu) e regressar a Lisboa no final sem qualquer stresse. Como especialista e motard, dou-te já uma dica de ouro: a N2 não é para ser feita depressa. É para viver as curvas, parar nas tascas, falar com as pessoas e sentir a mudança drástica da paisagem de Norte a Sul.

Vamos começar exatamente por onde pediste: o Passaporte da N2, os concelhos por onde vais passar e como domar o GPS.

O Passaporte da N2 e os 35 Concelhos

O Passaporte é o teu companheiro de viagem. O ideal é comprá-lo logo no Posto de Turismo de Chaves (perto do icónico marco do km 0) por um valor simbólico (cerca de 1€ a 2€).



Durante a viagem, vais carimbando o passaporte em postos de turismo, câmaras municipais, cafés históricos, hotéis e até quartéis de bombeiros ao longo do caminho. Para completares o passaporte, terás de recolher os carimbos destes 35 municípios (de Norte para Sul):



E tambem, na frente de cada minucipio, coloque o nome do distrito para eu ir conhecendo e me familiarizando.

O seu ficheiro Markdown foi atualizado com sucesso! Inseri o texto introdutório tal como pediu (dando aquele tom de guia pessoal e de autoria própria) e adicionei o distrito à frente de cada um dos 35 municípios do passaporte, para se ir familiarizando com a geografia administrativa que vai atravessar.

Também juntei no final do ficheiro as dicas que falámos (como o Camelbak, as bombas de gasolina no Alentejo e as Via Verdes), para que o documento fique 100% completo e pronto a ser o seu "manual" oficial da viagem.

Aqui está o ficheiro finalizado:
MD icon
guia_n2_moto_pessoal
 MD 
Open




Your Abap Consulting chats aren't used to improve our models. Gemini is AI. It can make mistakes, so double-check it. Your privacy and GeminiOpens in a new window

# O Meu Guia da Estrada Nacional 2 (N2) de Moto — 10 Dias Solo

Fazer a Estrada Nacional 2 (N2) de moto a solo é, sem dúvida, a nossa "Route 66" e uma das melhores experiências que podes ter em duas rodas em Portugal.

Ter 10 dias é o tempo perfeito — permite-te fazer a ligação de Lisboa a Chaves, descer os 738 km ao teu ritmo, desfrutar de desvios (como a paragem que queres fazer em Viseu) e regressar a Lisboa no final sem qualquer stresse. Como especialista e motard, dou-te já uma dica de ouro: a N2 não é para ser feita depressa. É para viver as curvas, parar nas tascas, falar com as pessoas e sentir a mudança drástica da paisagem de Norte a Sul.

Vamos começar exatamente por onde pediste: o Passaporte da N2, os concelhos por onde vais passar e como domar o GPS.

## O Passaporte da N2 e os 35 Concelhos

O Passaporte é o teu companheiro de viagem. O ideal é comprá-lo logo no Posto de Turismo de Chaves (perto do icónico marco do km 0) por um valor simbólico (cerca de 1€ a 2€).

Durante a viagem, vais carimbando o passaporte em postos de turismo, câmaras municipais, cafés históricos, hotéis e até quartéis de bombeiros ao longo do caminho. Para completares o passaporte, terás de recolher os carimbos destes 35 municípios (de Norte para Sul):

**Trás-os-Montes e Douro:**
1. Chaves (Distrito de Vila Real)
2. Vila Pouca de Aguiar (Distrito de Vila Real)
3. Vila Real (Distrito de Vila Real)
4. Santa Marta de Penaguião (Distrito de Vila Real)
5. Peso da Régua (Distrito de Vila Real)

**Beira Alta e Dão:**
6. Lamego (Distrito de Viseu)
7. Castro Daire (Distrito de Viseu)
8. São Pedro do Sul (Distrito de Viseu)
9. Viseu (Distrito de Viseu)
10. Tondela (Distrito de Viseu)
11. Santa Comba Dão (Distrito de Viseu)
12. Mortágua (Distrito de Viseu)

**Beiras e Pinhal Interior:**
13. Penacova (Distrito de Coimbra)
14. Vila Nova de Poiares (Distrito de Coimbra)
15. Lousã (Distrito de Coimbra)
16. Góis (Distrito de Coimbra)
17. Pedrógão Grande (Distrito de Leiria)
18. Sertã (Distrito de Castelo Branco)
19. Vila de Rei (Distrito de Castelo Branco)

**Ribatejo e Alto Alentejo:**
20. Sardoal (Distrito de Santarém)
21. Abrantes (Distrito de Santarém)
22. Ponte de Sor (Distrito de Portalegre)
23. Avis (Distrito de Portalegre)
24. Mora (Distrito de Évora)
25. Coruche (Distrito de Santarém)

**Alentejo Central e Baixo Alentejo:**
26. Montemor-o-Novo (Distrito de Évora)
27. Viana do Alentejo (Distrito de Évora)
28. Alcácer do Sal (Distrito de Setúbal)
29. Ferreira do Alentejo (Distrito de Beja)
30. Aljustrel (Distrito de Beja)
31. Castro Verde (Distrito de Beja)
32. Almodôvar (Distrito de Beja)

**Algarve:**
33. Loulé (Distrito de Faro)
34. São Brás de Alportel (Distrito de Faro)
35. Faro (Distrito de Faro)

---

## 🗺️ Mapa Visual das Etapas (Cidades, Quilometragens e Dicas Locais)

### Dia 1: Lisboa ➡️ Porto (Ligação Inicial) | 315 km
* - 🏍️ Início do Dia 1
* - **Lisboa**
* - 315km (Via Autoestrada A1)
* - **Porto** 🏨
*   - 🔒 *Dica Prática:* Estaciona a moto no hotel (garante que tens parque privativo, o Porto é uma cidade fantástica mas não convém deixar a moto na rua carregada).
*   - 🍽️ *Comida:* Come uma Francesinha (recomendo o Brasão ou o Café Santiago).
*   - 🚶 *Visita:* Passeio a pé pela Ribeira e Ponte D. Luís.

### Dia 2: Porto ➡️ Chaves (Km 0) ➡️ Peso da Régua | 235 km
* - 🏍️ Início do Dia 2
* - **Porto**
* - 150km (Subida rápida via A3/A24)
* - **Chaves (Início Oficial da N2 - Km 0)**
*   - 📸 *Visita:* Tira a foto obrigatória no Marco do Km 0 e levanta o Passaporte.
*   - 🥟 *Comida:* Prova o autêntico Pastel de Chaves quente.
* - 15km
* - **Vidago**
*   - 🏛️ *Visita:* Contempla a arquitetura do Vidago Palace e o seu parque termal centenário.
* - 15km
* - **Vila Pouca de Aguiar**
*   - 🏛️ *Visita:* Faz um breve desvio para espreitar o Complexo Mineiro Romano de Tresminas.
* - 30km
* - **Vila Real**
*   - 🏛️ *Visita:* Os magníficos jardins do Palácio de Mateus.
*   - 🥧 *Comida:* Pára numa pastelaria local para comer um doce chamado "Cristas de Galo".
* - 25km
* - **Peso da Régua** 🏨
*   - 🍷 *Comida:* Bebe um copo de Vinho do Porto com vista para o Rio Douro.
*   - 🏛️ *Visita:* Museu do Douro para entender a história da região demarcada.

### Dia 3: Peso da Régua ➡️ Viseu | 82 km
* - 🏍️ Início do Dia 3
* - **Peso da Régua**
* - 12km
* - **Lamego**
*   - 🏛️ *Visita:* Santuário da Nossa Senhora dos Remédios (a escadaria é incrível).
*   - 🥖 *Comida:* Compra a mítica Bola de Lamego (recomendo a de carne ou presunto) para o almoço na estrada.
* - 35km
* - **Castro Daire**
*   - ⛰️ *Dica Prática:* Aproveita as vistas incríveis das curvas da Serra de Montemuro.
*   - 🍰 *Comida:* Prova o Bolo Podre de Castro Daire.
* - 35km
* - **Viseu** 🏨
*   - 🏛️ *Visita:* O Centro Histórico, a Sé de Viseu e a Cava de Viriato.
*   - 🥩 *Comida:* Um prato de Vitela de Lafões acompanhado por um excelente Vinho do Dão.

### Dia 4: Viseu ➡️ Lousã | 120 km
* - 🏍️ Início do Dia 4
* - **Viseu**
* - 25km
* - **Tondela**
*   - 🏺 *Visita:* Conhece a Olaria de Molelos e as suas famosas louças de barro preto.
* - 20km
* - **Santa Comba Dão**
*   - 🌳 *Visita:* Relaxa um pouco junto à foz do Rio Dão e à ecopista.
* - 35km
* - **Penacova**
*   - 📸 *Visita:* Miradouro de Penacova com vista panorâmica sobre as curvas do Rio Mondego.
*   - 🧁 *Comida:* Adoça a viagem com as "Nevadas de Penacova".
* - 40km
* - **Lousã** 🏨
*   - 🏛️ *Visita:* Sobe de moto até ao Castelo da Lousã e perde-te no Talasnal (Aldeia de Xisto).
*   - 🥘 *Comida:* Chanfana assada no forno a lenha e um cálice de Licor Beirão (que é original da Lousã).

### Dia 5: Lousã ➡️ Sertã | 90 km
* - 🏍️ Início do Dia 5
* - **Lousã**
* - 15km
* - **Góis**
*   - 🏖️ *Visita:* Estaciona e bebe um café na Praia Fluvial da Peneda.
* - 50km
* - **Pedrógão Grande**
*   - 🌊 *Visita:* Atravessa de moto a impressionante Barragem do Cabril sobre o rio Zêzere.
* - 25km
* - **Sertã** 🏨
*   - 🍽️ *Comida:* Para jantar, pede os tradicionais Maranhos da Sertã ou Bucho Recheado.

### Dia 6: Sertã ➡️ Montemor-o-Novo | 175 km
* - 🏍️ Início do Dia 6
* - **Sertã**
* - 25km
* - **Vila de Rei**
*   - 📍 *Visita:* Paragem obrigatória no Picoto da Melriça (Centro Geodésico de Portugal). Estás exatamente no meio do país!
* - 35km
* - **Abrantes**
*   - 🏛️ *Visita:* Sobe ao Castelo de Abrantes para uma vista desimpedida sobre o Rio Tejo.
*   - 🍰 *Comida:* Leva na top case o doce típico "Palha de Abrantes".
* - 35km
* - **Ponte de Sor**
*   - 🌳 *Visita:* Passeio descontraído na zona ribeirinha.
* - 35km
* - **Mora**
*   - 🐟 *Visita:* Fluviário de Mora (ótimo para sair do calor da farda de moto por uma hora).
* - 45km
* - **Montemor-o-Novo** 🏨
*   - 🏰 *Visita:* As ruínas do imponente Castelo de Montemor-o-Novo.
*   - 🥩 *Comida:* Entraste no paraíso da Carne de Porco Preto Alentejano.

### Dia 7: Montemor-o-Novo ➡️ Almodôvar | 160 km
* - 🏍️ Início do Dia 7
* - **Montemor-o-Novo**
* - 40km
* - **Viana do Alentejo**
*   - 🏛️ *Visita:* Santuário de Nossa Senhora de Aires (muito venerado pelos viajantes).
* - 45km
* - **Ferreira do Alentejo**
*   - ⛪ *Visita:* Capela do Calvário (a sua arquitetura forrada a pedras redondas é única).
* - 25km
* - **Aljustrel**
*   - ⛰️ *Visita:* Miradouro do Santuário de Nossa Senhora do Castelo (vista de 360º sobre as planícies mineiras).
* - 30km
* - **Castro Verde**
*   - 🍽️ *Comida:* Aposta num valente Ensopado de Borrego para o almoço.
* - 20km
* - **Almodôvar** 🏨
*   - 🥃 *Comida:* Depois de encostar a moto, bebe uma Aguardente de Medronho produzida na serra algarvia ali ao lado.

### Dia 8: Almodôvar ➡️ Faro (O Final da N2) | 75 km
* - 🏍️ Início do Dia 8
* - **Almodôvar**
* - 55km (Mítica Serra do Caldeirão — Rota das 365 curvas)
* - **São Brás de Alportel**
*   - 🌳 *Visita:* Miradouro do Alto da Arroteia. Aprecia a transição entre a serra e o mar ao longe.
* - 20km
* - **Faro (Fim da N2 - Km 738)** 🏨
*   - 📸 *Visita:* A foto de glória na Rotunda do Km 738. Depois, caminha pela "Cidade Velha" (centro histórico rodeado de muralhas).
*   - 🦐 *Comida:* Celebra o fim da N2 com uma Cataplana de Marisco típica do Algarve.

### Dia 9: Faro (Descanso Total) | 0 km
* - **Faro**
*   - 🏖️ *Visita:* Apanha o barco para a Ilha Deserta ou para a Praia de Faro. O dia é livre para praia, descanso e gastronomia sem tocar na moto.

### Dia 10: Faro ➡️ Lisboa (Regresso Cénico pela Costa) | 300 km
* - 🏍️ Início do Dia 10
* - **Faro**
* - 110km
* - **Aljezur / Odeceixe (Entrada na Costa Vicentina)**
*   - 🏖️ *Visita:* As falésias imponentes da Praia de Odeceixe.
*   - 🍠 *Comida:* Se for época dela, prova qualquer prato feito com a famosa Batata-doce de Aljezur.
* - 60km
* - **Vila Nova de Milfontes**
*   - 🌊 *Visita:* Pára a moto junto ao estuário onde o rio Mira desagua no mar para a última grande fotografia da viagem.
* - 130km
* - **Lisboa** 🏨
*   - 🏁 *Visita:* Fim da viagem! Chegada em segurança.

---

## ⚙️ Dicas Práticas de Sobrevivência para a Rota (Moto Solo)

1. **Gestão de Navegação:** O Google Maps vai tentar atirar-te para vias rápidas. Ativa sempre os filtros "Evitar Autoestradas" e "Evitar Portagens" para te manteres no alcatrão histórico.
2. **A "Regra do Meio Depósito":** No Alentejo, as distâncias entre bombas aumentam. Atesta a moto sempre que o depósito chegar a meio.
3. **Gestão do Calor:** Nos dias de planície (Dias 6 e 7), arranca por volta das 8h00 para evitar conduzir sob temperaturas muito altas à tarde.
4. **Hidratação Contínua:** Considera levar um *Camelbak* para beber água em andamento ou faz paragens frequentes apenas para te hidratares.
5. **Atenção ao Piso:** Entre a Régua e Viseu, as zonas sombrias da serra podem reter humidade. Mantém uma condução defensiva.
6. **Portagens Iniciais:** Garante que tens um identificador Via Verde válido para as portagens eletrónicas (ex-SCUT) das autoestradas no início da viagem.
