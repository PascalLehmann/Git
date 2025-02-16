# How to write better git Commit

Thanks for the information of the website: [FreeCodeCamp](https://www.freecodecamp.org/news/how-to-write-better-git-commit-messages/)

Right now its only a bad german translation with an bad formatting


Bei der ersten Berührung mit Git ist es für Entwickler normalerweise so, dass sie sich mit dem Prozess unwohl fühlen.

Möglicherweise fühlen Sie sich unsicher, wenn Sie auf die Git-Commit-Nachricht stoßen, und wissen nicht, wie Sie die vorgenommenen Änderungen und deren Gründe richtig zusammenfassen sollen. Aber je früher Sie sich in Ihrer Karriere gute Commit-Gewohnheiten aneignen, desto besser.

Haben Sie sich schon einmal gefragt, wie Sie Ihre Git-Commit-Nachrichten verbessern können? In diesem Handbuch werden die Schritte zur Verbesserung Ihrer Commit-Nachrichten beschrieben, die Sie noch heute umsetzen können.

Dieser Artikel setzt voraus, dass Sie den grundlegenden Git-Workflow bereits kennen. Falls nicht, empfehle ich Ihnen, das Git-Handbuch durchzulesen .

Es ist auch wichtig zu beachten, dass Sie in erster Linie die Konventionen Ihres Teams befolgen sollten. Diese Tipps basieren auf Vorschlägen, die auf Forschung und allgemeinem Konsens der Community beruhen. Aber am Ende dieses Artikels haben Sie vielleicht einige Implementierungen vorgeschlagen, die den Arbeitsablauf Ihres Teams erleichtern können.

Ich glaube, Git betritt eine ganz andere Welt, sobald man anfängt, in Teams zu arbeiten – es gibt so viele tolle unterschiedliche Abläufe und Möglichkeiten, wie die Leute Code committen, Code teilen und Code zu Ihrem Repo hinzufügen können, ob Open Source oder Closed Source. – Scott Tolinski, Syntax.fm .

Warum sollten Sie bessere Commit-Nachrichten schreiben?
Ich fordere Sie auf, ein persönliches Projekt oder ein beliebiges Repository zu öffnen und git logeine Liste mit alten Commit-Nachrichten anzuzeigen. Die überwiegende Mehrheit von uns, die Tutorials durchgearbeitet oder schnelle Korrekturen vorgenommen haben, wird sagen: „Ja ... ich habe absolut keine Ahnung, was ich vor 6 Monaten mit ‚Fix-Stil‘ gemeint habe.“

Vielleicht sind Sie in einer professionellen Umgebung auf Code gestoßen, von dem Sie keine Ahnung hatten, was er tut oder wofür er gedacht ist. Sie tappten im Dunkeln, ohne Codekommentare oder einen nachvollziehbaren Verlauf und fragen sich sogar: „Wie hoch ist die Wahrscheinlichkeit, dass alles kaputt geht, wenn ich diese Zeile entferne?“

Zurück in die Zukunft
Indem Sie gute Commits schreiben, machen Sie sich einfach zukunftssicher. Sie könnten sich und/oder Ihren Kollegen stundenlanges Herumsuchen bei der Fehlerbehebung ersparen, indem Sie diese hilfreiche Beschreibung bereitstellen.

Die zusätzliche Zeit, die Sie aufwenden, um eine durchdachte Commit-Nachricht als Brief an Ihr potenzielles zukünftiges Ich zu schreiben, lohnt sich äußerst. Bei großen Projekten ist die Dokumentation für die Wartung unerlässlich.

Zusammenarbeit und Kommunikation sind in Entwicklungsteams von größter Bedeutung. Die Git-Commit-Nachricht ist hierfür ein Paradebeispiel. Ich empfehle dringend, eine Konvention für Commit-Nachrichten in Ihrem Team einzurichten, falls Sie noch keine haben.

Die Anatomie einer Commit-Nachricht
Basic:
git commit -m <message>

Im Einzelnen:
git commit -m <title> -m <description>

5 Schritte zum Schreiben besserer Commit-Nachrichten
Lassen Sie uns die vorgeschlagenen Richtlinien zusammenfassen:

Großschreibung und Zeichensetzung: Schreiben Sie das erste Wort groß und beenden Sie es nicht mit einem Satzzeichen. Denken Sie bei der Verwendung konventioneller Commits daran, nur Kleinbuchstaben zu verwenden.
Stimmung: Verwenden Sie in der Betreffzeile den Imperativ. Beispiel – Add fix for dark mode toggle state. Der Imperativ gibt den Ton an, als würden Sie einen Befehl oder eine Bitte erteilen.
Commit-Typ: Geben Sie den Commit-Typ an. Es wird empfohlen und kann sogar noch nützlicher sein, einen einheitlichen Satz von Wörtern zur Beschreibung Ihrer Änderungen zu haben. Beispiel: Bugfix, Update, Refactoring, Bump usw. Weitere Informationen finden Sie im Abschnitt zu konventionellen Commits weiter unten.
Länge: Die erste Zeile sollte idealerweise nicht länger als 50 Zeichen sein und der Textkörper sollte auf 72 Zeichen beschränkt sein.
Inhalt: Seien Sie direkt und vermeiden Sie Füllwörter und -phrasen in diesen Sätzen (Beispiele: obwohl, vielleicht, ich denke, irgendwie). Denken Sie wie ein Journalist.

So entdecken Sie den Journalisten in sich
Ich hätte nie gedacht, dass mein Nebenfach Journalismus meiner zukünftigen Karriere als Softwareentwickler zugute kommen würde, aber so ist es nun einmal!

Journalisten und Autoren stellen sich selbst Fragen, um sicherzustellen, dass ihr Artikel detailliert und unkompliziert ist und alle Fragen des Lesers beantwortet.

Beim Schreiben eines Artikels versuchen sie, die Fragen „Wer“ , „Was“ , „Wo“ , „Wann“ , „Warum “ und „Wie“ zu beantworten. Für Commit-Zwecke ist es am wichtigsten, das „Was“ und „Warum“ für unsere Commit-Nachrichten zu beantworten.

Um durchdachte Commits zu erstellen, sollten Sie Folgendes berücksichtigen:

Warum habe ich diese Änderungen vorgenommen?
Welche Wirkung haben meine Änderungen gehabt?
Warum war die Änderung notwendig?
Worauf beziehen sich die Änderungen?
Gehen Sie davon aus, dass der Leser nicht versteht, worum es bei dem Commit geht. Er hat möglicherweise keinen Zugriff auf die Story mit den detaillierten Hintergründen der Änderung.

Erwarten Sie nicht, dass der Code selbsterklärend ist. Dies ähnelt dem obigen Punkt.

Für Sie als Programmierer mag es offensichtlich erscheinen, wenn Sie etwas wie CSS-Stile aktualisieren, da es visuell ist. Sie wissen vielleicht genau, warum diese Änderungen zu diesem Zeitpunkt erforderlich waren, aber es ist unwahrscheinlich, dass Sie sich Hunderte von Pull Requests später daran erinnern werden, warum Sie das getan haben.

Machen Sie deutlich, warum diese Änderung vorgenommen wurde, und geben Sie an, ob sie für die Funktionalität entscheidend sein könnte oder nicht.

Die Unterschiede sind unten aufgeführt:

git commit -m 'Add margin'
git commit -m 'Add margin to nav items to prevent them from overlapping the logo'
Es ist klar, was davon für zukünftige Leser nützlicher sein wird.

Stellen Sie sich vor, Sie schreiben einen wichtigen, nachrichtlichen Artikel. Geben Sie eine Überschrift an, die zusammenfasst, was passiert ist und worauf es ankommt. Geben Sie dann im Hauptteil geordnet weitere Einzelheiten an.

In der Filmbranche heißt es oft „Zeigen, nicht erzählen“, wobei visuelle Elemente als Kommunikationsmedium verwendet werden, anstatt das Geschehen verbal zu erklären.

In unserem Fall heißt es: „ Erzählen , nicht [nur] zeigen“ – obwohl uns einige visuelle Hilfsmittel wie der Browser zur Verfügung stehen, ergeben sich die meisten Einzelheiten aus dem Lesen des physischen Codes.

Wenn Sie VSCode verwenden, laden Sie die Git Blame -Erweiterung herunter. Dies ist ein Paradebeispiel dafür, wann nützliche Commit-Nachrichten für zukünftige Entwickler hilfreich sind.

Dieses Plugin listet die Person auf, die die Änderung vorgenommen hat, das Datum der Änderungen sowie die inline kommentierte Commit-Nachricht.

Stellen Sie sich vor, wie nützlich dies bei der Fehlerbehebung oder beim Zurückverfolgen von vorgenommenen Änderungen sein könnte. Weitere lobende Erwähnungen zum Anzeigen historischer Git-Informationen sind Git History und GitLens .

Konventionelle Commits
Nachdem wir nun die grundlegende Commit-Struktur einer guten Commit-Nachricht behandelt haben, möchte ich konventionelle Commits vorstellen, um einige Einzelheiten zum Erstellen solider Commit-Nachrichten zu liefern.

Bei D2iQ verwenden wir Conventional Commit, eine bewährte Methode in Entwicklungsteams. Conventional Commit ist eine Formatierungskonvention, die eine Reihe von Regeln zur Formulierung einer konsistenten Commit-Nachrichtenstruktur bereitstellt, wie folgt:

<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
Der Commit-Typ kann Folgendes umfassen:

feat– Mit den Änderungen wird eine neue Funktion eingeführt
fix– Es ist ein Bugfix aufgetreten
chore– Änderungen, die sich nicht auf einen Fix oder ein Feature beziehen und keine Quell- oder Testdateien ändern (z. B. Aktualisieren von Abhängigkeiten)
refactor– überarbeiteter Code, der weder einen Fehler behebt noch eine Funktion hinzufügt
docs– Aktualisierungen der Dokumentation wie etwa der README-Datei oder anderer Markdown-Dateien
style– Änderungen, die die Bedeutung des Codes nicht beeinflussen, wahrscheinlich im Zusammenhang mit der Codeformatierung wie Leerzeichen, fehlende Semikolons usw.
test– einschließlich neuer oder korrigierender Prüfungen
perf– Leistungsverbesserungen
ci– kontinuierliche Integration im Zusammenhang
build– Änderungen, die das Build-System oder externe Abhängigkeiten betreffen
revert– macht ein vorheriges Commit rückgängig
Die Betreffzeile des Commit-Typs sollte vollständig in Kleinbuchstaben und mit einer Zeichenbegrenzung versehen sein, um prägnante Beschreibungen zu ermöglichen.

Der optionale Commit-Text sollte verwendet werden, um weitere Details bereitzustellen, die nicht in die Zeichenbeschränkungen der Betreffzeilenbeschreibung passen.

Es ist auch ein guter Ort, um BREAKING CHANGE: <description>den Grund für eine wesentliche Änderung innerhalb des Commits zu notieren.

Auch der Footer ist optional. Wir verwenden ihn, um beispielsweise auf die JIRA-Story zu verlinken, die mit diesen Änderungen geschlossen würde: Closes D2IQ-<JIRA #>.

Beispiel für ein vollständiges konventionelles Commit
fix: fix foo to enable bar

This fixes the broken behavior of the component by doing xyz. 

BREAKING CHANGE
Before this fix foo wasn't enabled at all, behavior changes from <old> to <new>

Closes D2IQ-12345
Um sicherzustellen, dass diese Commit-Konventionen für alle Entwickler einheitlich bleiben, kann die Lintierung von Commit-Nachrichten konfiguriert werden, bevor Änderungen hochgeladen werden können. Commitizen ist ein großartiges Tool, um Standards durchzusetzen, die semantische Versionierung zu synchronisieren und bietet weitere hilfreiche Funktionen.

Um die Übernahme dieser Konventionen zu erleichtern, ist es hilfreich, Richtlinien für Commits in eine Beitrags- oder README-Markdown-Datei in Ihren Projekten aufzunehmen.

Konventionelle Commits funktionieren besonders gut mit semantischer Versionierung (weitere Informationen finden Sie unter SemVer.org ), wo Commit-Typen die entsprechende Version für die Veröffentlichung aktualisieren können. Weitere Informationen zu konventionellen Commits finden Sie hier .

Commit-Nachrichtenvergleiche
Sehen Sie sich die folgenden Nachrichten an und prüfen Sie, wie viele der vorgeschlagenen Richtlinien in jeder Kategorie abgehakt werden.

Gut
feat: improve performance with lazy load implementation for images
chore: update npm dependency to latest version
Fix bug preventing users from submitting the subscribe form
Update incorrect client phone number within footer body per client request

Schlecht
fixed bug on landing page
Changed style
oops
I think I fixed it this time?
leere Commit-Nachrichten
Abschluss
Das Schreiben guter Commit-Nachrichten ist eine äußerst nützliche Fähigkeit, die Sie entwickeln sollten, und es hilft Ihnen, mit Ihrem Team zu kommunizieren und zusammenzuarbeiten. Commits dienen als Archiv für Änderungen. Sie können zu einem alten Manuskript werden, das uns hilft, die Vergangenheit zu entschlüsseln und in Zukunft begründete Entscheidungen zu treffen.

Es gibt bereits einen Satz vereinbarter Standards, an die wir uns halten können. Wenn sich Ihr Team jedoch auf eine Konvention einigt, die für künftige Leser aussagekräftig ist, wird es zweifellos langfristige Vorteile geben.

In diesem Artikel haben wir einige Taktiken kennengelernt, um unsere Commit-Nachrichten zu verbessern. Wie können diese Techniken Ihrer Meinung nach Ihre Commits verbessern?

Ich hoffe, Sie haben etwas Neues gelernt, danke fürs Lesen!
