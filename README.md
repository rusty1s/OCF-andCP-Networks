# Bachelor-Arbeit: Qualitative Semantiken für DAGs – ein Vergleich von OCF- und CP-Netzwerken

* **Universität**: Technische Universität Dortmund
* **Lehrstuhl**: Logik in der Informatik
* :paperclip: [PDF [0.4MB]](https://github.com/rusty1s/OCF-andCP-Networks/raw/master/thesis.pdf)
* :page_with_curl: [Publication](http://www.sciencedirect.com/science/article/pii/S0165011416300999)
* :movie_camera: [Slides](https://github.com/rusty1s/OCF-andCP-Networks/files/1299007/slides.pdf)

```
@mastersthesis{Fey2013,
  title={{Qualitative Semantiken f{\"u}r DAGs –- ein Vergleich von OCF- und CP-Netzwerken}},
  author={Matthias Fey},
  type={Bachelor-Thesis},
  school={Technische Universit{\"a}t Dortmund},
  year={2013},
}
```

oder

```
@article{EichhornFeyKernIsberner2016,
  title={{CP}- and {OCF}-networks -- a comparison},
  author={Christian Eichhorn and Matthias Fey and Gabriele {Kern-Isberner}},
  journal={Fuzzy Sets and Systems},
  year={2016},
  volume={298},
  pages={109--127},
  publisher={Elsevier Science Publishers},
  note={Special Issue on Graded Logical Approaches and Their Applications},
  address={Essex, UK},
}
```

## Einleitung

> Insofern sich die Gesetze der Mathematik auf die Wirklichkeit beziehen, sind sie nicht sicher. Und insofern sie sich sicher sind, beziehen sie sich nicht auf die Wirklichkeit. (Albert Einstein)

Viele tägliche Situationen sind von Unsicherheit und Ungenauigkeit geprägt. Ausdrücke und Worte der natürlichen Sprache können ungenau oder mehrdeutig sein. Es erscheint demnach ein sinnvolles Vorhaben, Unsicherheit und das Schlussfolgern in unsicheren Situationen zu modellieren und zu automatisieren.

Wir werden daher in dieser Arbeit zwei Repräsentanten für unsicheres Schließen kennenlernen, die auf der Grundlage von *Netzwerken* bzw. *gerichteten azyklischen Graphen (DAGs)* graphisch dargestellt werden können. Mit ihnen kann unsicheres Wissen repräsentiert werden, in dem Ereignissen in Abhängigkeit vom Eintreten anderer Ereignisse eine Plausibilität zugeordnet wird. Ebenso kann dann aus dem für am plausibelsten gehaltenen Wissen neues Wissen gewonnen werden.

* *Ordinale konditionale Funktions (OCF)*-Netzwerke beschreiben die entsprechenden Abhängigkeiten durch lokal bedingte Rangfunktionen, die den Ereignissen Ränge zuordnen, die den Grad der Überraschung repräsentieren, die mit dem Eintritt des Ereignisses verbunden sind. Ein Ereignis erscheint umso plausibler, je kleiner dessen Rang ist.
* *Ceteris Paribus (CP)*-Netzwerke ordnen Ereignissen unter dem Eintritt ihrer Vorereignisse eine Präferenz zu. Dadurch entsteht eine Präferenzrelation, aus der ein Wissenszustand gewonnen werden kann.

Wir stellen uns folgendes Szenario vor: An einem sonnigen Morgen wollen wir wie gewöhnlich die Zeitung lesen. Wir treten also vor die Tür um diese zu holen, aber zu unserem Bedauern stellen wir fest, dass sie zutiefst durchnässt ist. Für uns kommen nur zwei mögliche Schlüsse in Frage:

1. Es hat vor kurzem noch geregnet.
2. Der Sprinkler hat sich versehentlich angeschaltet.

Da wir an die Zuverlässigkeit von Maschinen glauben, könnten unsere Erwartungen an die beiden Netzwerke wie folgt aussehen:

* **OCF-Netzwerk:** Wir ordnen der Plausibilität des Regens einen Rang von 0 ein. Dass der Sprinkler sich selbstständig macht, halten wir allerdings für derart unplausibel, dass dessen Plausibilität nur einen Rang von 3 haben kann.
* **CP-Netzwerk:** Wir beurteilen die Präferenz der beiden Ereignisse zueinander und geben an: *Der Eintritt des Regens wird vor einem Defekt der Sprinkleranlage präferiert.*

CP-Netzwerke arbeiten mit der Präferenz zwischen Ereignissen ohne den Grad dieser in einem Zahlenwert festzuhalten, wohingegen OCF-Netze diesen Grad durch den Abstand der Ränge zueinander definieren. Durch die Präferenz-Ordnung der Ereignisse erhalten aber auch CP-Netzwerke eine Art Rang, der eine gewisse Ähnlichkeit von CP zu OCF-Netzen nicht ausschließt.

In dieser Arbeit wollen wir diesen möglichen Zusammenhang untersuchen und Gemeinsamkeiten und Unterschiede von CP- und OCF-Netzwerken ausarbeiten. Eventuell lässt sich ein Netzwerk in das andere überführen, gegebenenfalls sind sie sogar äquivalent. Die Feststellung, wann beziehungsweise unter welchen Bedingungen dies möglich sein könnte, ist Ziel dieser Arbeit.
