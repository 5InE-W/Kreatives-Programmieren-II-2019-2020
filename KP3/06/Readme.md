# 13.11.2019; Kreatives Programmieren 3

Modular/Trigger/Feedback

## Ziele/Ideen/Techniken

Ziel ist es Techniken und Arbeitsweisen analoger modularer Synthesizer in SuperCollider zu nutzen. Hierbei wollen wir stets direkt mit Signalen (äquivalent zu Spannungen bei analogen modularen Synthesizern) arbeiten. Feedback soll in irgendeiner Form als Gestaltungsmittel eingesetzt werden.

## Modular

* Was bedeutet Modular?
* UGens als Module im UGen-Graph
* LFOs
* Funktionen als Untermodule in der Klangsynthese
* SynthDefs als Module im Node Tree
* [Busse](http://doc.sccode.org/Classes/Bus.html)
* [Ndef](http://doc.sccode.org/Classes/Ndef.html)

## Trigger

* Was sind Trigger und wie funktionieren sie?
* Was kann ich mit Trigger anfangen?
* Wie lassen sich Trigger erzeugen?
* Ausblick Übung, Demand UGens: Server-seitige Patterns

## Feedback

* Was ist ein Feedback/Rückkopplung?
* Larsen effect ([Wiki](https://en.wikipedia.org/wiki/Audio_feedback))
* Feedback 'bändigen'; Regelsysteme
* Rekursion und Feedback
* Technische Probleme/Einschränkungen für Feedbacks in SuperCollider
* Feedback Quark ([FbC](http://quark.sccode.org/Feedback/Fb.html) und [FbNode](http://quark.sccode.org/Feedback/FbNode.html))
* Single-Sample-Feedback ([Example 1](https://github.com/supercollider/supercollider/blob/develop/examples/demonstrations/single_sample_feedback.scd), [Example 2](https://github.com/supercollider/supercollider/blob/develop/examples/demonstrations/single_sample_feedback_02.scd))
* Video Feedback [(Beispiel)](https://www.youtube.com/watch?v=WS8v6jKPP68)

## Quelltext

* [feedback_intro.scd](feedback_intro.scd)
* [modular_trigger_feedback.scd](modular_trigger_feedback.scd)

## Hausaufgabe

Baut mit Ndefs ein Netzwerk aus mehreren Syntheseprozessen die miteinander über Signale (ar, kr oder Trigger) interagieren. Das Netzwerk soll an mindestens einer Stelle ein Feedback enthalten. Das Feedback soll über einen Regelmechanismus verfügen - entweder manuell ([MouseX/Y](http://doc.sccode.org/Classes/MouseX.html), MIDI, NdefMixer, GUI ...) oder automatisch (z.B. [Amplitude](http://doc.sccode.org/Classes/Amplitude.html) oder zeitgesteuert via Envelopes, LFOs, etc.). Seid vorsichtig bei den Feedbacks! Am besten zumindest erstmal für den Anfang die Amplitude begrenzen (z.B. durch tanh).

Euer Netzwerk kann einem zeitlichen Ablauf folgen, sich periodisch wiederholen, ein komplexes Eigenleben haben oder als 'Instrument' mit Controllern (MIDI, NdefMixer, ...) gespielt werden.

Zur Gestaltung des Klangs stehen euch alle Möglichkeiten in SuperCollider zur Verfügung. Benutzt keine Patterns und erzeugt keine neuen Synth-Instanzen. Sequencing und zeitlicher Ablauf soll alles direkt auf Signalebene geregelt werden.

**Abgabe als Code per GitHub Repo und als Audioaufnahme per E-Mail bis zum 04.12.2019, Besprechung und Demonstration eurer Projekte am 27.11.2019.**

## Literatur

* [Scott Eric Peterson - Fun with Feedback (and SuperCollider)](https://scacinto.wordpress.com/2010/12/02/fun-with-feedback-and-supercollider/)
* ...

## Weiteres