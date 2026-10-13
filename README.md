# Algoritma Implementasi

## Deskriptif

1. Mulai
2. Masukan nilai mahasiswa
3. jika nilai lebih dari 80 , maka nilai mahasiwa tersebut adalah A
4. jika nilai kurang atau sama dengan 80 ,maka nilai B dan kalo tidak maka nilai C
5. selesai

## flowchart

```mermaid

flowchart TD

A@{ shape: circle, label: "Mulai" }
B@{ shape: lean-r, label: " nilai" }
C@{ shape: diamond, label: "nilai > 80" }
D@{ shape: diamond, label: "nilai <= 80" }
E@{ shape: lean-l, label: "nilai A" }
F@{ shape: lean-l, label: "nilai B" }
G@{ shape: lean-l, label: "nilai C" }
H@{ shape: dbl-circ, label: "Selesai" }


A-->B
B-->C
C--ya-->E
D--ya-->F
D--tidak-->G
C--tidak-->D
E-->H
F-->H
G-->H


```

## Pseude Code

DECLARE nilai : INTEGER

IF nilai > 80 THEN
OUTPUT "A"
ELSE
IF nilai <= 80 THEN
OUTPUT "B"
ELSE
OUTPUT "C"
ENDIF
ENDIF
