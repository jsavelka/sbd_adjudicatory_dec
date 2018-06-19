# **LLT Lab Protocol: Annotating the Boundaries of “Sentences”**

**Vern R. Walker, LLT Lab Director**\
**Research Laboratory for Law, Logic and Technology (LLT Lab)**\
**Maurice A. Deane School of Law at Hofstra University**\
**Fall 2017**

The following guidelines and examples govern our annotation of spans of text using the type “Sentence”.

# Part I: Guidelines [1]

> [FOOTNOTE 1] Normally, a Lab protocol contains more explicit and precise procedures for identifying an annotation type and its boundaries, but this protocol builds on an English writer’s intuitions about sentence content, grammar and sentence boundaries.

We adopt a fairly standard definition of a “sentence” from the linguistic theory that deals with written linguistic structures. A sentence is defined as a textual segment or span consisting of one or more words that are grammatically linked, and which expresses (in principle, and at least implicitly) a complete thought (even though it may be necessary to take context and conventions into account to understand that thought). Sentences might express a declarative statement, a question, an exclamation, a request, a command, or a suggestion.

Normally, an explicitly expressive sentence contains a grammatical subject and a grammatical predicate. [2] The grammatical subject is normally a noun phrase (a group of words that are in dependency relations with a single noun), and refers to the person, place or thing (including abstract things) that the sentence is about. The grammatical predicate is normally a verb phrase (a group of words that are in dependency relations with a single verb, which in turn refers to an action, process or state). An example of a normal sentence structure is “The veteran filed a claim for disability benefits,” where “the veteran” is the grammatical subject and “filed a claim for disability benefits” is the grammatical predicate.

> [FOOTNOTE 2] It is worth noting also that statutes and regulations sometimes disregard normal grammar. For example, see the second definition under 42 C.F.R. § 489.24 (b) (“Comes to the emergency department means ...”). In that definition, there is a single noun phrase (as grammatical subject) followed by a list of four verb phrases (functioning as grammatical predicates), but some verb phrases on the list are followed by additional sentences before the next list item. So one complete sentence has other sentences interspersed within it. In order for the listed verb phrases to make sense, we have to annotate the entire complex as a single sentence (and ignore the fact that other sentences are embedded within it). Despite the unusual syntax, the human reader makes sense of the whole provision (largely by ignoring the usual grammatical rules).

Not all sentences are explicit in what they express. An example of a one-word sentence with implicit meaning is “Yes.” when it is an answer to the interrogatory sentence “Did you seek medical attention for your condition?” In context, the sentence “Yes.” has the same meaning as the explicit sentence “I did seek medical attention for my condition.” Other examples of spans that we will annotate as sentences (see the examples below in List C) are:

* Data fields, such as “Decision Date: 03/28/17” - which we understand as having the same meaning as “This decision was issued on March 28, 2017.”
* Headings, such as “FINDINGS OF FACT” - which we understand as having meaning similar to “The sentences in the following section state the findings of fact of the tribunal.”
* List numbers or letters, such as “1.” - which in context we understand as meaning “The following is the first item on the list.”

In selecting the span of characters that we annotate as type “Sentence”, be sure to highlight and annotate the *entire* sentence. There are normally several linguistic features to guide you. Any **white space** before the sentence *is not part of* the sentence span. Normally a sentence in English begins with a **capital letter** (i.e., the first character within the span selected as being a sentence is normally a capital letter). The **punctuation** at the end of the sentence *is part of* the sentence span. In the case where a **quotation mark** (whether single or double) precedes the initiating capital letter or follows the normal sentence-ending punctuation mark, then the quotation mark should be included within the sentence boundaries. Similarly, if a parenthesis precedes the initiating capital letter or follows the normal sentence-ending punctuation mark, then the parenthesis should be included within the sentence boundaries. But no annotation span should start or end with a white space.

Sentences in English normally end with one of three sentence-ending punctuation characters: a period (also called a “full stop”), a question mark, and an exclamation mark. We seldom see exclamation marks (“!”) in legal texts, but they do occur occasionally. In BVA decisions, you will sometimes see sentences ending in a question mark, especially in a section of the decision specifying issues to be addressed on remand. Normally, sentences end with a period (full stop) - although periods also cause extensive segmentation error, because many periods in legal texts do not signal the end of a sentence (e.g., periods within abbreviations or citations). You should assume that a sentence never ends with a comma, a semicolon, or a colon (although in the case of a colon, we will see an exception in the examples below when the colon introduces a new paragraph consisting of an itemized list or a block quote, and should be regarded as ending a sentence).

# Part II: Lists of Examples (Organized into 3 lists)

## List A: Normal Form

A span of characters is a “normal form” if we are *highly confident* that it constitutes an annotation of the type “Sentence”, and this confidence is *based on some evidence or feature from the span text itself (the "linguistic cue")*. Also, a sentence in “normal form” has a certain *fixed format or pattern*, which we find *recurring* numerous times. These should be the easiest types of sentences for computer software to identify.

In the case of annotations for the type “Sentence”, the normal form is a grammatical subject consisting of a noun phrase followed immediately by a grammatical predicate consisting of a verb phrase. The noun phrase and verb phrase can contain subordinate clauses, provided the sentence as a whole is relatively easy to parse by parts of speech.

#### EXAMPLES

> The Veteran's chronic adjustment disorder with depressed and anxious features is related to service.\
[NOTE: the noun phrase is “the Veteran’s chronic adjustment disorder with depressed and anxious features”; the verb phrase is “is related to service”.]

> The Veteran does meet the criteria for a diagnosis of posttraumatic stress disorder (PTSD).\
[NOTE: the noun phrase is “the Veteran”; the verb phrase is “does meet the criteria for a diagnosis of posttraumatic stress disorder (PTSD)”.]

> A disability which is aggravated by a service-connected disability may be service-connected.\
[NOTE: the dependent clause “which is aggravated by a service-connected disability” modifies “disability” and is part of the noun phrase that is the grammatical subject of the sentence. The verb phrase is “may be service-connected”.]

## List B: Linguistic Transforms of Normal Forms

A span of text that is a “linguistic transform” of a normal form is one for which we are also *highly confident* that it constitutes an annotation of the type “Sentence”, a confidence based on some evidence or feature from the span text itself (the "linguistic cue"). However, while a sentence in normal form has a straightforward format or pattern of &lt;grammatical subject noun phrase&gt;&lt;grammatical predicate verb phrase&gt;, *a “linguistic transform” has a more complex linguistic pattern* that is in principle transformable into sentences that do have normal forms. There might be some linguistic rules that would make it easier for computer software to identify such forms. So here we are looking for merely grammatical transformations of the normal form for sentences.

#### EXAMPLES

> Consequently, as outlined in a February 2013 Formal Finding, the RO requested information from the Joint Services Records Research Center (JSRRC) and the US Army Crime Records Center; however, those sources provided negative responses for the requested date range.\
[NOTE: This sentence has a complex grammatical structure that departs from the simple normal form. It can be parsed into two independent clauses, the second of which has a sentence normal form. The first clause, however, contains the grammatical subject in the middle of the clause.]

> Establishment of service connection for PTSD in particular requires: (1) medical evidence diagnosing PTSD; (2) credible supporting evidence that the claimed in-service stressor actually occurred; and (3) medical evidence of a link between current symptomatology and the claimed in-service stressor.\
[NOTE: This is a single sentence that contains a numbered list. This is to be distinguished from the numbered lists discussed in List C.]

> See, e.g., Young v. McDonald, 766 F.3d 1348, 1353 (Fed. Cir. 2014) ("PTSD is not the type of medical condition that lay evidence . . . is competent and sufficient to identify.").\
[NOTE: This example illustrates that citation sentences are indeed sentences, even though they do not have the normal form of a sentence. But they do express complete thoughts in highly encoded form. This citation sentence, for example, means the following: “The decision by the U.S. Court of Appeals for the Federal Circuit in 2014 named ‘Young v. McDonald’ contains, at page 1353 of volume 766 of the third series of the Federal Reporter, the sentence ‘PTSD is not the type of medical condition that lay evidence . . . is competent and sufficient to identify.’.” The fact that the Bluebook of formats for legal citations is so thorough leads us to put citation sentences in List B (linguistic transforms of normal forms) instead of in List C (aberrant forms of normal forms).]

## List C: Aberrant Forms of Normal Forms

A span of text can have a very unusual linguistic structure, but we are *still confident* (but maybe not “highly confident”) that it constitutes an annotation of the type “Sentence”. This confidence might be based more on the context than on linguistic cues within the span itself (e.g., co-references with words or phrases in other sentences). These we will have to study to determine what reasons we can give for annotating them as sentences.

There are certain classes of examples on which we can generalize.

### Case Names in Document Titles

Case names in document titles express a single thought, and are best treated as a single sentence. This is true regardless of how the case name is formatted in a particular document (e.g., spread over several lines). Because of the peculiar sentence structure, it would be a rather distinctive type of sentence from which we could mine more information later.

#### EXAMPLE

> SOUNDEXCHANGE, INC. Plaintiff v. MUZAK, LLC Defendant.

### Headings or Organizational Sentences

Some spans of text that we will annotate as “sentences” organize the text (chunk it into meaningful segments). We will annotate them as “sentences” (see the guidelines at the beginning of this protocol).

#### EXAMPLES

> ISSUES (or THE ISSUE)\
INTRODUCTION\
FINDINGS OF FACT\
CONCLUSIONS OF LAW\
REASONS AND BASES FOR FINDINGS AND CONCLUSIONS\
ORDER\
REMAND

### Data-Field Sentences

Some spans of text that we will annotate as “sentences” provide a data field and a value (see the guidelines at the beginning of this protocol). They implicitly assert the value of the data field.

#### EXAMPLES

> Citation Nr: 1710389\
Decision Date: 03/28/17\
Archive Date: 04/11/17\
DOCKET NO.  12-12 279\
Veteran represented by:	 Veterans of Foreign Wars of the United States

> RYAN T. KESSEL\
Veterans Law Judge, Board of Veterans' Appeals&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Department of Veterans Affairs\
[NOTE: As a matter of pure convention, for BVA decisions we will annotate the signature block of the decision as *two* sentences, the first stating the judge’s name, and the second stating the judge’s title (even if “Department of Veterans Affairs” is on a separate line in the decision).]

### Numbered or Lettered Lists

Numbered or lettered lists require special treatment, and the treatment depends on whether the list items are themselves sentences or not.

*If the list items are themselves sentences* (including headings that we are annotating as sentences), then we will annotate the number or letter itself (the number or letter of the list item) as a sentence, and the sentence that is the list item as another sentence. The rationale is that we would create problems for machine learning or for our own understanding if we include the list-item number (“1.”) as part of the sentence that is the list item. The “1.” expresses a thought separate from the sentence it introduces. The numbering of the list could change, but the role and meaning of each sentence on the list would remain the same. We don’t want an ML program treating “1.” as part of the sentence it introduces, or trying to POS parse the sentence including the “1.” within the sentence boundaries.

#### EXAMPLES

> FINDINGS OF FACT\
(1)  The Veteran does meet the criteria for a diagnosis of posttraumatic stress disorder (PTSD).  
(2)  The Veteran's chronic adjustment disorder with depressed and anxious features is related to service.\
[NOTE: This passage contains 5 sentences. The heading “FINDINGS OF FACT” is a sentence (see the guideline above on headings). The two numbers introducing the list items (“1.” and “2.”) are each sentences. Then there are two list items, which are each sentences in normal form.]

> I. Laws and Regulations\
[NOTE: A numbered or lettered heading should be two sentences. In the example above, “I.” should be one sentence (making a statement about where the heading is in a sequence of headings). The heading itself should be one sentence (its meaning normally unaffected by its order in the sequence of headings).]

*If the list items are not themselves sentences*, then there is an overall sentence that includes the list items, and the list numbers or letters occur within that overall sentence. In such a case, there is only one sentence. Although the sentences of statutes and regulations are often very long and complex, we try to follow this same guideline in annotating them (whether we are annotating the statute or regulation directly, or we are annotating a block quotation of the statute or regulation within a judicial decision).

#### EXAMPLES

>Establishment of service connection for PTSD in particular requires: (1) medical evidence diagnosing PTSD; (2) credible supporting evidence that the claimed in-service stressor actually occurred; and (3) medical evidence of a link between current symptomatology and the claimed in-service stressor.\
[NOTE: This example is a single sentence that contains three phrases that happen to be numbered; it is therefore a single sentence. This example is also given in List B above, as a linguistic transform of a normal form.]

> [3] These factors are:
(1) the nature and circumstances of the offense and the history and characteristics of the defendant;\
(2) the need for the sentence imposed\
(A) to reflect the seriousness of the offense, to promote respect for the law, and to provide just punishment for the offense;\
(B) to afford adequate deterrence to criminal conduct;\
(C) to protect the public from further crimes of the defendant; and\
(D) to provide the defendant with needed educational or vocational training, medical care, or other correctional treatment in the most effective manner;\
(3) the kinds of sentences available;\
(4) the kinds of sentence and the sentencing range established for . . . the applicable category of offense committed by the applicable category of defendant as set forth in the guidelines . . .\
(5) any pertinent policy statement . . . issued by the Sentencing Commission . . . subject to any amendments made to such policy statement by act of Congress. . . .\
(6) the need to avoid unwarranted sentence disparities among defendants with similar records who have been found guilty of similar conduct; and\
(7) the need to provide restitution to any victims of the offense.

> 18 U.S.C. § 3553(a).\
[NOTE: This long passage is a single endnote in a judicial decision (for annotation of endnotes, see the guideline for endnotes below). By the guidelines on endnotes, “[3]” would be one sentence. Since “These factors are:” is text introducing a numbered or lettered list, it would be a separate sentence ending in a colon (see the guideline for colons below). The outline list that follows the colon is taken from 18 U.S.C. § 3553(a). It is a single sentence (with embedded ellipses, and phrases connected by semi-colons), and is therefore one long sentence. The citation at the end is also a single sentence. So this entire passage consists of 4 sentences: [3], “These factors are:”, 18 U.S.C. § 3553(a), and the very complex sentence in between.]

> [13] "4. Assuming it is decided that segregation in public schools violates the Fourteenth Amendment\
"(a) would a decree necessarily follow providing that, within the limits set by normal geographic school districting, Negro children should forthwith be admitted to schools of their choice, or\
"(b) may this Court, in the exercise of its equity powers, permit an effective gradual adjustment to be brought about from existing segregated systems to a system not based on color distinctions?\
"5. On the assumption on which questions 4 (a) and (b) are based, and assuming further that this Court will exercise its equity powers to the end described in question 4 (b),\
"(a) should this Court formulate detailed decrees in these cases;\
"(b) if so, what specific issues should the decrees reach;\
"(c) should this Court appoint a special master to hear evidence with a view to recommending specific terms for such decrees;\
"(d) should this Court remand to the courts of first instance with directions to frame decrees in these cases, and if so what general directions should the decrees of this Court include and what procedures should the courts of first instance follow in arriving at the specific terms of more detailed decrees?"\
[NOTE: This passage consists of five sentences. “[13]” is a sentence, because it is the footnote/endnote indicator. The long quotation is broken into four sentences. Because the quotation is a (partial) list with complete sentences as list items, the list numbers “4.” and “5.” are each sentences. Finally, the two items in the list are themselves sentences (interrogative sentences).]

### Page Numbers

The page numbers of a reporter service occur in one of two ways. First, if they occur outside of normal sentences, then it seems best to annotate them as separate sentences. In the passage below, the character sequence “*1163” means “This is where page 1163 begins in the Federal Reporter, Third Series.” This passage then contains 3 sentences, the middle one being the sentence “*1163”:

> He contends that to do so would be, in effect, to report himself for the new crime of being found in the country after deportation. *1163 See United States v. Pina-Jaime, 332 F.3d 609, 612 (9th Cir.2003) (holding that an alien need not have reentered the United States illegally to be convicted of being "found in" the country illegally).

It makes sense to treat such an occurrence of “*1163” as a separate sentence, for many of the same reasons given above for treating the itemizing numbers of lists as sentences and for treating headings as sentences. (Incidentally, the auto-SBD annotated the above passage as 3 sentences.)

Second, a page number could occur embedded within a normal sentence, as in the following example:

> The record in this case shows no attempt, by either the Probation Officer or sentencing court, to justify this *1162 sweeping condition.

In such a situation, we don't want to split the normal sentence into parts just because a page number happens to occur inside it.

### Endnotes or Footnotes

The in-text indicators for endnotes or footnotes (usually numbers, but sometimes letters or other characters) should be included within the boundaries of the sentence where they occur. Sometimes this is embedded within the span, and sometimes after the sentence-ending punctuation.

#### EXAMPLES

> Barsumyan was arrested and indicted for one count of producing, using, and trafficking in a counterfeit credit card, 18 U.S.C. § 1029(a)(1), and three counts of possession of device-making equipment, 18 U.S.C. § 1029(a)(4).[2]

> Barsumyan gave the Agent a “skimming device,[1] and asked her to covertly “skim” the hotel guests' credit cards when they registered.

If the endnotes themselves appear as a numbered list, then we follow the guideline for numbered lists, so the following would be four sentences (with “[4]” being the first sentence, meaning “The fourth endnote is the following.”, followed by two normal sentences and a citation sentence):

> [4] Both wireless telephones and credit cards are considered “access devices” for these purposes. The cloning of wireless telephones was considered particularly serious because cloned cell phones are commonly used by drug dealers and other criminals to evade surveillance. See 144 Cong. Rec. S3021 (1998) (statement of Sen. Leahy); 143 Cong. Rec. S2655 (1997) (statement of Sen. Kyl).

Footnotes would follow the same guideline as for endnotes, even if the numbered list does not occur in one place in the document.

### Colons Ending Sentences

There is one situation in which we will regard the colon as sentence-ending punctuation, whereas presumptively it is not. This situation is when the colon is the last punctuation mark in a paragraph - i.e., the colon is followed immediately by a line break. A colon is therefore treated as sentence-ending punctuation if, but only if, it is followed immediately by a line break.

There are several reasons for deciding this. Although the use of a colon can be highly stylistic, in general an author uses a colon instead of a period to express that what goes before the colon is meaningfully related to what comes after – that they are in effect connected into one thought. That is why the colon is presumptively not sentence-ending punctuation. However, an author may use a colon followed immediately by a line break to introduce a block quote or a numbered or lettered list of items. In such a situation, if we do not end the sentence with the colon, where would we end it? After the entire block quote (which may contain multiple sentences or paragraphs)? The quoted sentence(s) should be annotated independently, and parsed separately, without being part of the sentence that introduces the block quote. Similarly, a stand-alone itemized list should be annotated independently of the introducing sentence.

Unfortunately, a colon followed immediately by a line break might separate a grammatical subject from a list of grammatical verbs, as we often find in statutory or regulatory texts. The convention we adopt here is a compromise between the desire to have first-pass segmentation that is as non-semantic as possible (as with tokenization) and the desire to preserve intact all propositional content in the process of segmentation. We stress that this is a first-pass compromise. After this initial segmentation into sentences, on subsequent passes we can parse the spans of text before and after a “&lt;colon&gt;&lt;line-break&gt;” to determine if they are semantically related, and if warranted we can then annotate the entire passage (also) as a single, overall sentence.

#### EXAMPLES

> For example, in a June 1977 service personnel record a counselor opined that:\
\
I have personally interviewed this SM and found him to have a good attitude towards the Army.  However, he has a serious academic problem.\
[NOTE: This example contains 3 sentences. The first sentence ends with a colon: “For example, in a June 1977 service personnel record a counselor opined that:”. The second and third sentences follow normal rules.]

> Accordingly, the case is REMANDED for the following action:\
\
(1) When disability ratings and effective dates have been determined for all service-connected disabilities, to include those granted herein, and all development that the RO deems necessary is undertaken, the Veteran's request for a TDIU should be readjudicated.\
[NOTE: This example contains 3 sentences: “Accordingly, the case is REMANDED for the following action:”; “1.”; and the sentence beginning with “When disability …”. For the reason that “1.” is annotated as a sentence, see the guidelines above for numbered lists.]

> MILAN D. SMITH, JR., Circuit Judge:\
[NOTE: this sentence providing the judge’s name introduces the entire opinion.]

> It has been shown that this opinion could not hold because: "there [is] not enough support in evidence. This must be so."\
[NOTE: this example contains two sentences. The first sentence is: &lt;SEN&gt;It has been shown that this opinion could not hold because: "there [is] not enough support in evidence.&lt;/SEN&gt;. The colon is not immediately followed by a line break, so the sentence does not end with the colon. The second sentence is: &lt;SEN&gt;This must be so."&lt;/SEN&gt;. It might seem undesirable to include the first double-quotation mark in one sentence, and the second double-quotation mark in the following sentence. On the other hand, this preserves valuable semantic information, which we can then use on subsequent passes to annotate the entire intact quotation as a “Quotation” type.]

### Ellipses
*If the ellipsis occurs within a sentence span* and it indicates missing words from within that sentence, then the ellipsis should be included in the overall sentence span.

#### EXAMPLE

> ... the conferee's objective was to limit the grandfather to their existing services in the same transmission medium 152*152 and to any new services in a new transmission medium where only transmissions similar to their existing service are provided.\
[NOTE: this passage was the beginning of a block quotation.]

*If the ellipsis occurs between sentences*, then such an ellipsis should be annotated as a separate sentence. The rationale is that it provides coded information (“Sentences have been deleted”), and we don’t want the ellipsis to be parsed within the complete sentences that precede and follow it.

#### EXAMPLES

> (3) The defendant shall comply with the immigration rules and regulations of the United States, and, if deported from this country, either voluntarily or involuntarily, not reenter the United States illegally. The defendant is not required to report to the Probation Office while residing out-side *1157 of the United States; however, within 72 hours of release from any custody or any reentry to the United States during the period of Courtordered supervision, the defendant shall report for instructions to the United States Probation Office. . . .\
. . .\
(5) The defendant shall not access or possess any computer or computer-related devices in any manner, or for any purpose, unless approved in advance by the Probation Officer.\
[NOTE: This passage contains 7 sentences (incidentally the auto-SBD did in fact annotate this passage as 7 sentences). Besides the regular sentences, one ellipsis occurs after a completed sentence and another one occurs between paragraphs in the block quote.]

> The court concluded that, under the circumstances of this case, the presumptive privilege was overcome by the Special Prosecutor's prima facie "demonstration of need sufficiently compelling to warrant judicial examination in chambers . . . ."\
	[NOTE: The final ellipsis should be a sentence on its own (with the double-quotation mark falling within the boundary of the ellipsis sentence).]

### Phrases Functioning as Sentences

Sometimes phrases function as complete sentences, as though there is an implicit ellipsis. We will annotate them as complete sentences.

#### EXAMPLE

> Entitlement to service connection for a psychiatric disorder.\
[NOTE: this list item is a noun phrase only, but because it occurs in a list with the heading “ISSUES”, we understand it to mean the sentence “An issue is this case is whether there is entitlement to service connection for a psychiatric disorder.”]

### Grammatical or Typographical Errors

It occasionally happens that the human author of the document omits punctuation. If we can still determine from context and content that the span of text is a sentence (often because of what comes after it, together with its content), we should still annotate it as a sentence. For example, the first example below should be annotated as a sentence, despite the missing period at the end, because this span was followed by a normal sentence.

#### EXAMPLES

> 38 U.S.C.A. § 1111 (West 2014)\
[NOTE: the omitted final period is inferred because this text is followed by a normal sentence.]

> Federal Rule of Criminal Procedure 52(b) states that "[a] plain error that affects substantial rights may be considered even though it was not brought to the court's attention." (Emphasis added).\
[NOTE: This passage should be annotated as two sentences. I think that the proper punctuation for the second sentence is “(Emphasis added.)” - ending in a parenthesis, not a period.]
 
### Parentheticals within Sentences
 
 Even if a parenthetical that occurs within a sentence contains one or more separate sentences, the sentences within the parentheses are not annotated separately.
 
#### EXAMPLE
 
 Id. at 576, 128 S. Ct. 558; see also id. at 575, 128 S. Ct. 558 ("The District Court began by properly calculating and considering the advisory Guidelines range. It then addressed the relevant § 3553(a) factors.").[6]\
[NOTE: This is in fact a single sentence, even though the parenthetical contains two normal sentences within quotation marks.]

### Other Aberrations (that do not form a general category)

#### EXAMPLES

{ADD AS DISCOVERED}

