# Debugging

Why does the board only add horizontal but not vertical battleships?

ved denne opgave kører jeg programmet til et bestemt punkt. her stepper jeg in i debug mode for at se hvordan metoden bliver kaldt. når jeg så finder punktet hvor programmet laver skibet, markere jeg selve koden for at se hvad programmet gør. dette gør jeg flere gange og opdager hurtigt at resultatet er 0 hele tiden. derefter prøver jeg at evaluate hvor jeg + med 1. derefter kan jeg se at programmet genere tilfældige 1'ere og 0'ere.

dette retter jeg i programmet og det fikser problemet.


Why do we never get message Ship sunk! when log output shows 3 direct hits?

her gør jeg på samme måde hvor jeg laver breakpoint ved BattleshipGame.play da det er der problemet opstår. jeg stepper in helt ind til metoden hvor jeg kan se hvad der sker med skibet når den bliver ramt. da der står  " > " betyder det at betoden først bliver sandt hvis hitcount bliver over 3. derfor tilføjer jeg = så den ser således ud: >=  dette tester jeg også virker programmet

Why do we sometimes see java.lang.ArrayIndexOutOfBoundsException?

for at finde dette tilføjer vi en breakpoint hvor vi skriver java.lang.ArrayIndexOutOfBoundsException. dette fører os til problemet direkte når den kommer frem. så man kører programmet i debug indtil det kommer frem. programmet kender kun værdierne 0-9 som 1-10 og derfor forstår den ikke at 10 er udover dens grænser. derfor tilføjer man en loop kode som gør at programmet tester om den er mellem værdierne programmet kender
