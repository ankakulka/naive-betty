---
title: "Test"
date: 2022-12-29T15:16:02+01:00
draft: true
# bookComments: false
# bookSearchExclude: false
mermaid: true
---

He visited this country also with a view of catching horse-whales,
which had bones of very great value for their teeth, of which he
brought some to the king. ...  The best whales were catched in his
own country, of which some were forty-eight, some fifty yards long.
He said that he was one of six who had killed sixty in two days."
--OTHER OR OCTHER'S VERBAL NARRATIVE TAKEN DOWN FROM HIS MOUTH BY
KING ALFRED, A.D. 890.

"And whereas all the other things, whether beast or vessel, that
enter into the dreadful gulf of this monster's (whale's) mouth, are
immediately lost and swallowed up, the sea-gudgeon retires into it in
great security, and there sleeps." --MONTAIGNE.

"Let us fly, let us fly!  Old Nick take me if is not Leviathan
described by the noble prophet Moses in the life of patient Job."
--RABELAIS.



{{< columns >}} <!-- begin columns block -->
# Left Content
"The great Leviathan that maketh the seas to seethe like boiling
pan." LORD BACON'S VERSION OF THE PSALMS.

# Mid Content
"Touching that monstrous bulk of the whale or ork we have received
nothing certain.  They grow exceeding fat, insomuch that an
incredible quantity of oil will be extracted out of one whale."
--IBID.  "HISTORY OF LIFE AND DEATH."

# Right Content
"The sovereignest thing on earth is parmacetti for an inward bruise."
KING HENRY.
{{< /columns >}}



{{< details title="THE FAERIE QUEEN" open=true >}}

"Which to secure, no skill of leach's art
Mote him availle, but to returne againe
To his wound's worker, that with lowly dart,
Dinting his breast, had bred his restless paine,
Like as the wounded whale to shore flies thro' the maine.
{{< /details >}}



{{< tabs "uniqueid" >}}
{{< tab "HOBBES'S LEVIATHAN" >}} By art is created that great Leviathan, called a Commonwealth or
State--(in Latin, Civitas) which is but an artificial man.{{< /tab >}}
{{< tab "PILGRIM'S PROGRESS" >}} Silly Mansoul swallowed it without chewing, as if it had been a
sprat in the mouth of a whale.{{< /tab >}}
{{< tab "PARADISE LOST" >}} That sea beast
Leviathan, which God of all his works
Created hugest that swim the ocean stream. {{< /tab >}}
{{< /tabs >}}




# Mermaid Chart

[MermaidJS](https://mermaid-js.github.io/) is library for generating svg charts and diagrams from text.

{{< hint info >}}
**Override Mermaid Initialization Config**

To override the [initialization config](https://mermaid-js.github.io/mermaid/#/Setup) for Mermaid,
create a `mermaid.json` file in your `assets` folder!
{{< /hint >}}

## Example

{{< columns >}}
```tpl
{{</*/* mermaid [class="text-center"]*/*/>}}
stateDiagram-v2
    State1: The state with a note
    note right of State1
        Important information! You can write
        notes.
    end note
    State1 --> State2
    note left of State2 : This is the note to the left.
{{</*/* /mermaid */*/>}}
```

<--->

{{< mermaid >}}
stateDiagram-v2
    State1: The state with a note
    note right of State1
        Important information! You can write
        notes.
    end note
    State1 --> State2
    note left of State2 : This is the note to the left.
{{< /mermaid >}}

{{< /columns >}}


{{ if (.Params.mermaid) }}
{{<mermaid>}}
graph TD;
  A-->B;
  A-->C;
  B-->D;
  C-->D;
{{</mermaid>}}
<script async src="https://unpkg.com/mermaid@8.2.3/dist/mermaid.min.js"></script>
{{ end }}