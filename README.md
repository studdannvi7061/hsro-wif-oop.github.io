# Pflichtmodul: Objektorientierte Programmierung (OOP)

**(formerly known as 'Programmieren 2')**

_Pflichtmodul im [Bachelorstudiengang Wirtschaftsinformatik](https://www.th-rosenheim.de/technik/informatik-mathematik/wirtschaftsinformatik-bachelor/) an der [Hochschule Rosenheim](https://www.th-rosenheim.de)._

## Organisatorisches

**Vorlesungstermin**: Montags, 11:45-13:15 A3.13

**Übungen**: Dienstags, 2./3./4. Stunde, S1.31; Tutor: Daniel Herzinger

**Kommunikation**: via [Mattermost](https://inf-mattermost.th-rosenheim.de/wif-oop-ss19/channels/town-square) ([einschreiben](https://inf-mattermost.fh-rosenheim.de/signup_user_complete/?id=ptti4zza5fyqbg76jnz1jkjuia))

**Coding Contest**: via [domjudge](http://domjudge.inf.fh-#rosenheim.de) (**Achtung**: nur übers `fhintern` Netz #(WLAN oder Kabel), oder über das VPN)

**Wichtige Termine**:

- **??. April:** Prüfungsanmeldung im OSC
- **13. Mai:** Einführung in das Contestsystem (persönliche Anwesenheit erforderlich!)


## Leistungsnachweis

- schriftliche Prüfung (SP, 90 Minuten) am Ende des Semesters


## Empfohlene Literatur

- [Offizielle Java Dokumentation](https://docs.oracle.com/javase/9/)
- Ullenboom, C: [Java ist auch eine Insel](https://www.amazon.de/Java-auch-eine-Insel-Java-Entwickler/dp/3836258692/), 2017. ([Online verfügbar!](http://openbook.galileocomputing.de/javainsel))
- Bäckmann, M: [Objektorientierte Programmierung für Dummies](https://www.amazon.de/Objektorientierte-Programmierung-Dummies-Marcus-B%C3%A4ckmann/dp/3826629841/), 2002. _Das Buch ist für C++, die Methodik aber identisch zu Java._
- Gamma, E et al.: [Design Patterns](https://www.amazon.com/Design-Patterns-Object-Oriented-Addison-Wesley-Professional-ebook/dp/B000SEIBB8), 1994. (Das Buch ist in englischer und deutscher Fassung in der Bibliothek vorhanden).


## Inhalt
- **18. März: Professionelle Softwareentwicklung** ([Einführung](00-einfuehrung/), [Skript](01-professionelle-softwareentwicklung/), [Übung 1](https://github.com/hsro-wif-oop/tutorial), [Übung 2](https://github.com/hsro-wif-oop/example))

	Nach ein paar organisatorischen Dingen widmen wir uns dem Handwerkszeug professioneller Softwareentwicklung.
	Wir wiederholen Spezifikation mit UML, Versionierung mit git, Tests und Ausnahmebehandlung.

- **25. März: Liste als sequenzielle Datenstruktur** ([Skript](02-linked-list/), [Übung](https://github.com/hsro-wif-oop/oop-uebung01))

	Bisher haben wir größere Mengen von gleichen Objekten in Feldern (Arrays) gespeichert, welche aber in ihrer Größe in Java unveränderlich sind.
	Wir erarbeiten uns nun mithilfe der Objektorientierung eine dynamische Datenstruktur, welche nach Bedarf wachsen und schrumpfen kann und so Daten effizient verwaltet.

- **1. April: Set als Menge eindeutiger Elemente** ([Skript](/03-tree-set/), [Übung](https://github.com/hsro-wif-oop/uebung02))

	Eine Liste speichert Daten sequenziell ab, achtet dabei aber nicht auf Duplikate.
	Ein _Set_ (aus dem engl. _set:_ Menge, Gruppe) ist ein Containertyp, welcher der mathematischen Menge nachempfunden ist: jedes Element kann genau einmal vorkommen, und es gibt keine Ordnung (Reihenfolge); ein Element ist entweder enthalten oder nicht.
	Zur Implementierung lernen wir den Binärbaum kennen, eine weitere wichtige Datenstruktur der Informatik.

- **8. April: Generics** ([Skript](/04-generics/), [Übung](https://github.com/hsro-wif-oop/uebung03))

	Bisher waren die Containerklassen entweder für genau einen Datentyp, oder für die `Object`, welche für jedes Objekt verwendet werden kann.
	_Generics_ erlauben es nun mit beliebigen, _aber festgelegten,_ Datentypen zu arbeiten.
	Wir lernen ausserdem die Interfaces `Comparable` und `Comparator` kennen.

- **15. April: Iteratoren** ([Skript](/05-iterator/), [Folien](/05-iterator/slides/), [Übung](https://github.com/hsro-wif-oop/uebung04))

	Arrays und Listen verfügen über einen Indexoperator (`[]` bzw. `get(int)`), welcher verwendet werden kann um alle Elemente zu besuchen.
	Der _Iterator_ abstrahiert dieses Prinzip: Bereitgestellt vom Container selbst, ist er ein Hilfsobjekt mit dem jedes Element des Containers besucht werden kann.

- 22./23. April: Vorlesung und Uebungen entfallen wg. Ostern

- **29. April: Map als generischer assoziativer Container** ([Skript](/06-map/), [Folien](/06-map/slides/), [Übung](https://github.com/hsro-wif-oop/uebung05))

	Eine Liste ist sequenziell mit potentiellen Duplikaten, ein Set ist duplikatfrei, aber ohne Reihenfolge.
	Eine _Map_ (aus dem engl. _map_: Abbildung) ist ein assoziativer Container, welcher einem Schlüssel (_key_) eindeutig einen Wert (_value_) zuordnet.

- **6. Mai: Rekursion** ([Skript](/07-rekursion/), [Folien](/07-rekursion/slides/), [Übung](https://github.com/hsro-wif-oop/uebung06))

	Ging es um das Abarbeiten von Daten bzw. Implementieren von Algorithmen, so gingen wir bisher meist iterativ vor, also mit `for` bzw. `while`.
	Rekursion ist nun ein Mittel, bei der eine Methoden sich selbst wieder (mit veränderten Argumenten) aufrufen, und so ohne `for` bzw. `while` auskommen.

- **13. Mai: [Annotationen](/08-annotationen/slides/) und [Einführung in domjudge wg. Coding Contest](/psta/slides/)**

	Nach einem kurzen Exkurs zum Thema Annotationen und deren Einsatzgebieten gibt es eine Einführung in den Coding Contest.

- **20. Mai: Sortieren** ([Skript](/09-sortieren/), [Übung](https://github.com/hsro-wif-oop/uebung07))

	Gewappnet mit Datenstrukturen, Iteration und Rekursion erarbeiten wir Algorithmen zum Sortieren von Daten.
	Wir begegnen wieder den Interfaces `Comparable<T>` und `Comparator<T>`, welche die Vergleichsoperation abstrahieren.

- **27. Mai: Datenverarbeitung (Teil 1)** ([Skript](/10-datenverarbeitung/), [Folien](/10-datenverarbeitung/slides/), [Übung](https://github.com/hsro-wif-oop/uebung08))

	Wir lernen die Containerklassen der Java Bibliothek kennen um effizient und übersichtlich Daten zu verarbeiten.
	Klassischerweise ist die Datenverarbeitung hier in vier Schritten zu machen: filtern, sortieren, abbilden und reduzieren.

- **3. Juni: Datenverarbeitung (Teil 2)**

- _10./11. Juni: Vorlesung und Übungen entfallen_

- **17. Juni: Vererbung** ([Folien](/11-vererbung/vererbung-1.pdf), [Übung](https://github.com/hsro-wif-oop/uebung09))

	Bisher waren unsere Klassenbeziehungen vorwiegend strukturell bzw. funktional: Ein Monat besteht aus Tagen, ein Auto aus Bauteilen, usw.
	_Vererbung_ erlaubt es nun verwandschaftliche Beziehungen zu modellieren, und so Gemeinsamkeiten in Oberklassen zu bündeln.
	So sind z.B. sowohl Audis als auch BMWs im Grunde genommen _Autos_, doch gibt es sowohl geteilte Eigenschaften als auch spezielle.

- **24. Juni: Abstrakte Basisklassen** ([Folien](/11-vererbung/vererbung-2.pdf), [Übung](https://github.com/hsro-wif-oop/uebung10))

	Abstrakte Basisklassen sind ein weiteres Syntaxmittel, um verwandschaftliche Beziehungen zu beschreiben.
	Da abstrakte Klassen nicht instanziiert werden können, sind sie im Grunde ähnlich zu Schnittstellen (_Interfaces_), erlauben aber genauere Modellierung der Sichtbarkeiten.

- **1. Juli: Parallele Verarbeitung** ([Folien](/12-parallel/slides/), [Skript](/12-parallel/), [Übung](https://github.com/hsro-wif-oop/uebung11))

	Folgten unsere Programme bisher einem vorgesehenen Ablaufplan, so erlauben _Threads_ die parallele Verarbeitung von Daten.
	Wir beginnen mit der Basisimplementierung und erarbeiten einige knifflige Situationen.

- **8. Juli: Zusammenfassung** ([Folien](/13-zusammenfassung/slides/))
