---
layout: post
title: Hardware-Wissen
---

## Die Kontrolleinheit (CU)

Die Kontrolleinheit ist für die Zusammenarbeit einzelner Teile des Prozessors verantwortlich. Der Kern der Kontrolleinheit ist das Befehlsregister. Da Register die schnellsten Speicher in einem Prozessor sind und aufgrund ihrer Leistungsfähigkeit nur wenig Platz (meist 32- oder 64-Bit) bieten, sind im Befehlsregister nur die nötigsten Befehle wie z.B. arithmetische oder logische Befehle vorhanden. Ein Computer mit diesen „reduzierten“ Befehlsregistern wird übrigens RISC  genannt.
Ein bestimmter Befehl im Befehlsregister besteht aus dem jeweiligen Operationscode, der beschreibt, welche Operation genau vorgenommen wird, welche und wie viele Operanden dafür benötigt werden und wo das Ergebnis abgelegt wird. Es wird nun mit der sogenannten „fetch“-Operation, die standardmäßig in jedem Register vorhanden ist, auf die Arbeitsspeicher-adresse, die im Befehlszähler steht, zugegriffen, danach wird der Befehls-zähler inkrementiert. Dabei wird der Operationscode aus dem Befehlsregister geladen. Sogenannte general-purpose Register speichern dabei die verschiedenen Operanden, die für die Operation benötigt werden, bzw. das Ergebnis, welches bei der Operation entsteht. Der Befehlsdecodierer generiert aus den Operationscodes der Befehle Steuersignale, die dann über die Operationssteuerung an die Arithmetisch-logische-Einheit (ALU) weitergeleitet werden.
