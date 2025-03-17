
# Multisensory Haptic Interactions - Understanding the Sense and Designing for it


## Zusammenfassung der wichtigsten Inhalte

1. **Grundlagen der Haptik**
	Der haptische Sinn setzt sich aus taktilen (Hautrezeptoren) und kinästhetischen (Muskeln und Gelenke) Wahrnehmungen zusammen. Haptische Schnittstellen sind Geräte, die dem Nutzer über Berührung Informationen vermitteln. Es gibt energetisch passive (z. B. mechanische Knöpfe) und energetisch aktive Systeme (z. B. vibrotaktile Rückmeldungen oder Kraftfeedback).
2. **Herausforderungen im haptischen Design**
	Haptische Wahrnehmung ist vielseitig, aber schwerer zu standardisieren als visuelle oder auditive Interfaces. Es gibt große individuelle Unterschiede in der Wahrnehmung und Interpretation haptischer Signale.	Die Integration haptischer Elemente in Multimodal-Interfaces ist komplex.
3. **Multimodale Interaktion mit Haptik**
	Haptische Signale können als verstärkende, komplementäre oder führende Elemente in Kombination mit anderen Sinnesmodalitäten genutzt werden.	Anwendungen reichen von Navigation über immersive VR bis hin zu teleoperierten chirurgischen Systemen. Haptische Interaktion kann als Benachrichtigung, Führung oder Informationsdarstellung dienen.
4. **Designprozess für haptische Medien**
	Das Design folgt einem iterativen Prozess mit den Phasen Browse – Sketch – Refine – Share.
	Sketching in Haptik ist besonders herausfordernd, da taktile Konzepte schwer visuell darstellbar sind. Kollaborative Tools und ==Versionierung== spielen eine wichtige Rolle bei der Weiterentwicklung haptischer Erlebnisse.
5. **Werkzeuge & Methoden für das Haptic Design**
	Bibliotheken und Frameworks helfen bei der Gestaltung haptischer Effekte. Rapid Prototyping mit Arduino und Open-Source-Hardware vereinfacht die Entwicklung. Autorentools ermöglichen die intuitive Gestaltung haptischer Sequenzen ohne Programmierkenntnisse.
	

## Notizen zu wichtigen Stellen

### Designprozess
Der Designprozess für haptische Medien wird als **iterativer, kreativer Prozess** beschrieben, der sich an klassischen Designmethoden orientiert. Ein zentraler Bezugspunkt ist der **Design Funnel von Bill Buxton**, der verschiedene Phasen von der Ideenfindung bis zur finalen Umsetzung umfasst.

 **Vier Hauptphasen des haptischen Designprozesses**

1. **Browse (Inspiration & Recherche)**    
    - Sammlung von bestehenden haptischen Konzepten und Technologien.
    - Herausforderung: **Wie speichert und klassifiziert man haptische Erlebnisse?**
    - Mangel an standardisierten Begriffen und Notationen für haptische Konzepte.
2. **Sketch (Schnelles Experimentieren & Prototyping)**    
    - In der visuellen Gestaltung ist Sketching einfach, aber in Haptik schwer umzusetzen.
    - **Haptic Sketching** wird als Methode genutzt: Einsatz physischer Materialien oder schneller Prototyping-Techniken (z. B. Arduino, vibrotaktile Module).
    - Herausforderung: **Fehlende abstrakte Darstellungsmöglichkeiten für haptische Ideen**.
3. **Refine (Iterationen & Optimierung)**    
    - Anpassung und Weiterentwicklung der haptischen Designs basierend auf Nutzerfeedback.
    - Herausforderung: **Haptische Iteration ist langsam**, da viele Änderungen an Hardware & Software gekoppelt sind.
    - Lösung: Entwicklung von **Tools zur Echtzeit-Anpassung haptischer Parameter**.
4. **Share (Teilen & Feedback einholen)**
    - Austausch von haptischen Designs ist schwierig, da keine **einheitlichen Formate oder Plattformen** existieren.
    - Vergleich mit visuellen Medien: Während Bilder oder Videos leicht geteilt werden können, erfordert Haptik physische Hardware oder spezielle Simulations-Software.
    - Lösung: **Haptic Libraries & Online-Plattformen** für kollaboratives Arbeiten.

> [!PDF|] [[Multisensory Haptic Interactions - Understanding the Sense and Designing for it.pdf#page=21&selection=9,1,23,10|Multisensory Haptic Interactions - Understanding the Sense and Designing for it, p.21]]
> > Making Haptic Media How do we translate knowledge of the physical and semantic haptic design space into compelling, coherent, and learnable haptic media, given the many and particular challenges it presents? The answer is a robust and flexible process. We draw upon a design thinking approach, often described as a funnel of idea candidates wherein the designer iteratively generates, refines and narrows down multiple ideas in parallel until a final, well-developed, and trusted design concept remains (Figure 3.4. We look now at how generic forms of design thinking must be adapted when applied to haptics, and offer several different schemas for approaching haptic design (including those introduced earlier for the user’s view of haptic sensations see Section 3.3.3). We close with an inventory of current haptic design tools and techniques
> 
> 

### Sketching
 --> schnelles Iterieren, verschiedene Konzepte erforschen
- spielt vor allem zu Beginn des Designprozesses und für diese Arbeit eine wichtige Rolle

> [!PDF|] [[Multisensory Haptic Interactions - Understanding the Sense and Designing for it.pdf#page=23&selection=28,0,32,20|Multisensory Haptic Interactions - Understanding the Sense and Designing for it, p.23]]
> > Sketching allows people to form abstracted, partial views of a problem or design, iterate very rapidly and explore concepts. This is mostly heavily used early in design, and plays a role in collaboration (discussed more under “Share” below). Of course, such a central technique is used as a key way of thinking about experience design [Buxton 2007]
> 
> 

Problem: Im haptischen Anwendungsfall fehlen zwei der wichtigsten Features für diese Phase:

**Abstrahierung und Mehrdeutigkeit (Abstraction and Ambiguity)**
Im Gegensatz zu visuellen oder auditiven Medien gibt es **keine standardisierte Notation oder universelle Symbolik** für haptische Signale. In der visuellen Gestaltung können Designer Skizzen oder Wireframes erstellen, um Ideen grob darzustellen. Für haptische Empfindungen fehlt eine vergleichbare, abstrakte Darstellungsform. Haptische Designer **müssen oft direkt Prototypen erstellen**, um Ideen zu testen, da eine abstrakte Vorabdarstellung schwierig ist.

> [!PDF|] [[Multisensory Haptic Interactions - Understanding the Sense and Designing for it.pdf#page=23&selection=37,0,45,44|Multisensory Haptic Interactions - Understanding the Sense and Designing for it, p.23]]
> > With respect to abstractability, we note that haptics suffers from a dearth of notation. Sketching of physical devices or interfaces is well supported, with paper and pencil and innumerable software assists. Sketching motion, and in particular showing what is or might be felt in, say, a vibrotactile experience, is trickier. While we can sketch a visual interface and look at it, it is much harder to sketch a haptic sensation and imagine it without feeling it.

**Schnelle Iteration (Rapid Iteration)**
Visuelle Interfaces lassen sich einfach anpassen, während haptische Prototypen oft physische Änderungen oder Neuprogrammierung erfordern.
Die Verbindung zwischen Hardware (z. B. vibrotaktile Aktuatoren) und Software erfordert eine enge Abstimmung, was Änderungen erschwert.

Dieses Problem wurde meiner Meinung nach bereits in ersten Schritten in CollabJam gelöst:
- schnelles und direktes Ändern einer vibrotaktilen Sequenz
- die geänderte Sequenz kann direkt abgespielt und erlebt werden 
	(ohne Änderungen an der Hardware vorzunehmen - Abgesehen von möglichen Positionsänderungen der Aktoren)

Die Benutzeroberfläche nutzt Elemente, die Nutzende vielleicht bereits aus DAWs kennen, und orientiert sich sowohl in der Bedienung als auch in der Bearbeitung von Sequenzen an etablierten Konzepten aus dem musikalischen Umfeld. Dies umfasst beispielsweise die Anordnung von Spuren, die visuelle Darstellung von Sequenzen sowie Interaktionsmechanismen wie das Setzen, Verschieben und Modifizieren von Events, wodurch ein vertrauter und intuitiver Workflow geschaffen wird.

Was anscheinend auch ein erfolgreicher Ansatz ist (Wie an anderen Softwarelösungen zu betrachten, welche einen vergleichbaren Ansatz verfolgen)

> [!PDF|] [[Multisensory Haptic Interactions - Understanding the Sense and Designing for it.pdf#page=29&selection=34,21,36,78|Multisensory Haptic Interactions - Understanding the Sense and Designing for it, p.29]]
> >  The Vibrotactile Score [Lee et al. 2009] is built around a musical schema and was shown to be generally preferable to programming in C and XML, but required familiarity with musical notation [Lee and Choi 2012].

# Sketching User Experiences: Getting the Design Right and the Right

## Eigenschaften einer Skizze

### Attribute von Sketches

- **Schnell & zeitnah**: Sketches sollten schnell zu erstellen sein und zum richtigen Zeitpunkt verfügbar sein.
- **Kostengünstig & entsorgbar**: Sie sollen keine hohen Kosten verursachen und leicht verworfen werden können.
- **Plentiful (Vielfältig & in Serie gedacht)**: Ein einzelner Sketch hat meist wenig Bedeutung – erst in einer **Serie** entsteht ein sinnvoller Kontext.
- **Klar definierter Stil**: Sketches folgen Konventionen (z. B. grobe Linien, geringe Details), um als solche erkannt zu werden.
- **Flüssige Gestik & Minimalismus**: Sie sind nicht präzise wie technische Zeichnungen, sondern offen und explorativ.
- **Angemessene Detailtiefe & Verfeinerung**: Sie enthalten nur das Wesentliche und suggerieren nicht mehr Präzision, als in der aktuellen Phase erforderlich ist.
- **Mehrdeutigkeit & Offenheit**: Sie sollen verschiedene Interpretationen ermöglichen und neue Perspektiven eröffnen.
### Sinn von Sketches

- **Erkunden statt Bestätigen**: Sketches sind Werkzeuge zur Ideenfindung, nicht zur endgültigen Festlegung.
- **Kommunikationshilfe**: Sie fördern Diskussionen und Interaktionen innerhalb des Designprozesses.
- **Flexibilität & Anpassbarkeit**: Sketches verhindern, dass frühzeitig eine fertige Lösung angenommen wird, was den kreativen Prozess behindern könnte.
- **Richtige Balance in der Detailtreue**: Zu wenig Details erschweren das Verständnis, zu viele lassen es wie eine endgültige Lösung wirken.

> [!PDF|] [[Sketching-userexperiences_gettingthedesignrightandtherightdesign.pdf#page=112&selection=12,0,58,30|Sketching-userexperiences_gettingthedesignrightandtherightdesign, p.112]]
> > Quick: A sketch is quick to make, or at least gives that impression. Timely: A sketch can be provided when needed. Inexpensive: A sketch is cheap. Cost must not inhibit the ability to explore a concept, especially early in the design process. Disposable: If you can’t afford to throw it away when done, it is probably not a sketch. The investment with a sketch is in the concept, not the execution. By the way, this doesn’t mean that they have no value, or that you always dispose of them. Rather, their value largely depends on their disposability. Plentiful: Sketches tend not to exist in isolation. Their meaning or relevance is generally in the context of a collection or series, not as an isolated rendering. Clear vocabulary: The style in which a sketch is rendered follows certain conventions that distinguish it from other types of renderings. The style, or form, signals that it is a sketch. The way that lines extend through endpoints is an example of such a convention, or style. Distinct gesture: There is a fluidity to sketches that gives them a sense of openness and freedom. They are not tight and precise, in the sense that an engineering drawing would be, for example. Minimal detail: Include only what is required to render the intended purpose or concept. Lawson (1997, p. 242) puts it this way, “ … it is usually helpful if the drawing does not show or suggest answers to questions which are not being asked at the time.” Superfluous detail is almost always distracting, at best, no matter how attractive or well rendered. Going beyond “good enough” is a negative, not a positive.
> 
>

> [!PDF|] [[Sketching-userexperiences_gettingthedesignrightandtherightdesign.pdf#page=114&selection=12,0,31,61|Sketching-userexperiences_gettingthedesignrightandtherightdesign, p.114]]
> > Appropriate degree of refinement: By its resolution or style, a sketch should not suggest a level of refinement beyond that of the project being depicted. As Lawson expresses it, “ … it seems helpful if the drawing suggests only a level of precision which corresponds to the level of certainty in the designer’s mind at the time.” Suggest and explore rather than confirm: More on this later, but sketches don’t “tell,” they “suggest.” Their value lies not in the artifact of the sketch itself, but in its ability to provide a catalyst to the desired and appropriate behaviours, conversations, and interactions. Ambiguity: Sketches are intentionally ambiguous, and much of their value derives from their being able to be interpreted in different ways, and new relationships seen within them, even by the person who drew them.

--> Design is **compromise**

# Schneider2017 - Haptic experience design - What hapticians do and where they need help

## Hindernisse im haptischen Design (1.2 Obstacles to Design)

- Begrenztes Wissen & wenig verfügbare Inhalte
	Es gibt nur wenige etablierte Methoden oder Standards für haptisches Design.

> [!PDF|] [[Schneider2017 - Haptic experience design - What hapticians do and where they need help.pdf#page=2&selection=392,1,409,8|Schneider2017 - Haptic experience design - What hapticians do and where they need help, p.6]]
> > Haptic content remains scarce and design knowledge is limited.

- Technologische Hürden
	- Unterschiedliche Hardware-Plattformen erschweren die Entwicklung.
	- Kommunikationsverzögerungen (Latenz) beeinflussen die haptische Qualität.

> [!PDF|] [[Schneider2017 - Haptic experience design - What hapticians do and where they need help.pdf#page=2&selection=410,1,445,1|Schneider2017 - Haptic experience design - What hapticians do and where they need help, p.6]]
> > Some issues are technological, such as highly variable hardware platforms and communications latency (Kaaresoja et al., 2014)

- Menschliche Faktoren
	- Individuelle Unterschiede in der Wahrnehmung von haptischen Reizen.
	- Einfluss von Alter (sensorischer Abbau) und persönlichen Erfahrungen auf die Interpretation von Haptik.
	- Enge Verbindung zwischen haptischer Wahrnehmung und anderen Sinnesmodalitäten.

> [!PDF|] [[Schneider2017 - Haptic experience design - What hapticians do and where they need help.pdf#page=2&selection=447,0,619,7|Schneider2017 - Haptic experience design - What hapticians do and where they need help, p.6]]
> > Other issues are human-centered, arising from individual user characteristics in perception and preferences: low-level perceptual variation (Lofvenberg and Johansson, 1984), responses to programmed (Levesque et al., 2011) and natural (Hollins et al., 2000) textures, sensory declines due to aging (Stevens, 1992; Stevens and Choo, 1996), and varied interpretation and appreciation of haptic effects and sensations (Seifi and MacLean, 2013; Seifi et al., 2015) – often because of personal experience (Schneider and MacLean, 2014), or of the close relationship between touch and other senses.
> 

# Schneider - Tactile Animation by Direct Manipulation of Grid Displays

## Wichtige Anforderungen für haptische Design-Tools (LR Description)

**Echtzeit-Wiedergabe (Real-Time Playback)**    
    - Schnelles Prototyping ist essenziell, um VT-Sensationen iterativ zu verbessern.
    - Direkte haptische Rückmeldung während der Gestaltung beschleunigt den Designprozess.
    - Herausforderung: Zu viel Echtzeit-Feedback kann zu kognitiver Überlastung führen.
**Laden, Speichern & Bearbeiten (Load, Save, Manipulate)**
    - Dauerhafte Speicherung von Designs ermöglicht langfristige Projekte und Kollaboration.
    - Klare Datenstrukturen erleichtern Funktionen wie Undo/Redo, um Experimente zu unterstützen.
**Bibliothek von Effekten (Library of Effects)**
    - Gespeicherte haptische Effekte helfen Designern, bewährte Muster wiederzuverwenden.
    - Verhindert, dass frühere Konzepte unnötig neu entwickelt werden müssen.
**Gerätekonfiguration (Device Configuration)**    
    - Haptische Tools müssen unterschiedliche Hardware unterstützen.
    - Konfigurationsdateien ermöglichen die Anpassung von Aktuatoren, Positionen & Algorithmen.
**Mehrere Kanäle & Effekt-Kombinationen (Multiple Channels & Combination of Effects)**    
    - Möglichkeit, mehrere haptische Effekte gleichzeitig oder sequentiell zu kombinieren.
    - Oft dargestellt als Timeline, um zeitliches Verhalten von Effekten zu visualisieren.
**Visuelle & direkte Steuerungsmetaphern (Visual/Direct Control Metaphor)**    
    - Intuitive Darstellung von Geräten & Aktuatoren, um haptische Reize direkt zu manipulieren.
    - Ermöglicht räumliches Denken über das haptische System.
**Audio-/Visueller Kontext (Audio/Visual Context)**    
    - Haptik wird stark von anderen Sinnen beeinflusst.
    - Zusätzliche Audio- & visuelle Hinweise helfen, haptische Effekte besser wahrzunehmen.
**Nutzerfeedback (User Feedback)**    
    - A/B-Tests & Nutzer-Feedback sind entscheidend für die Bewertung und Verbesserung haptischer Designs.
    - Ermöglicht, die Benutzererfahrung gezielt zu optimieren.

> [!PDF|] [[Schneider - Tactile Animation by Direct Manipulation of Grid Displays.pdf#page=3&selection=0,2,63,101|Schneider - Tactile Animation by Direct Manipulation of Grid Displays, p.3]]
> > LR Description LR1 Real-Time Playback [21, 26] Rapid prototyping is essential for working with VT sensations, especially in absence of objective metrics. Feeling a sensation at design time allows iteration to converge faster to better results. However, too real-time can cause split attention. LR2 Load, save, manipulate [14, 24, 26] A persistent object model is essential for sensation editing over longer projects and sharing with other designers or across devices. Well-defined actions upon a data structure also facilitates features like undo that support experimentation. LR3 Library of effects [6, 9, 23, 31, 32] A library of saved sensations is an important feature used in previous haptic authoring tools, providing inspiration and preventing designers from re-inventing the wheel. LR4 Device configuration [17–19, 23] Because of the many types of haptic devices, a general tool must be able to understand different devices. Lightweight configuration files are common in the literature, allowing users to select specific hardware, specify location and type of actuators, and choose a rendering algorithm. LR5 Multiple channels & combination of effects [6, 23, 25, 31, 32] Being able to display multiple effects simultaneously, or combine effects via superposition or concatenation, is essential for expanding the design space. This is typically represented in a timeline, which represents the temporal behaviour of any objects. LR6 Visual/direct control metaphor [3, 17, 23] Most previous tools consider each actuator separately. When thinking semantically about a spatial system, a direct view of the device and actuator layout is critical for direct manipulation. LR7 Audio/visual context [17, 21, 32] Haptic perception depends greatly on additional senses [8]. By providing audio and visual feedback, these effects can be mitigated and the designer can experience haptic sensations in context. LR8 User Feedback [26,32] Receiving feedback from users, either by demonstration or A/B testing, is extremely valuable.

