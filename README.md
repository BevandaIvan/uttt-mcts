# uttt-mcts
Monte Carlo Tree Search implementation for playing Ultimate Tic Tac Toe. School project. Project is in Croatian.

Ovaj je računalni program koji igra ultimativni križić-kružić moj nastavni projekt iz informatike. 

Ultimativni križić-kružić kompleksnije je proširenje standardne igre križić-kružić. Ako ne znate pravila, možete više saznati na poveznici https://en.wikipedia.org/wiki/Ultimate_tic-tac-toe. Igra se pokazala teškom za naučiti za računala jer nema heurističku evaluacijsku funkciju tj. teško je odrediti tko je u boljoj poziciji iz nekog stanja igrače ploče. Šah, recimo, ima takvu funkciju i zbog toga je lakše napisati računalni program koji igra šah. Tehnike poput minimaxa ne postižu zadovoljavajuće rezulatate u ovoj igri, pa sam morao koristiti MCTS (Monte Carlo Tree Search) algoritam. Više o tom algoritmu možete naučiti na poveznici https://en.wikipedia.org/wiki/Monte_Carlo_tree_search.

Ploča je numerirana kao šahovska ploča tj. horizontalno slovima A-I s lijeva na desno, a vertikalno brojevima od 1 do 9 od dolje prema gore. Pri pokretanju, model će prvo upitati težinu koju želite. Težina predstavlja broj iteracija MCTS algoritma. Trebala bi biti u desetcima tisuća da bi model igrao donekle dobro. *Ako je težina ispod 100, može doći do grešaka!* Nakon što je odabrana željena težina, možete jednostavno upisati potez koji ste odlučili odigrati, a model će ispisati potez koji želi napraviti. Za sada, ploču treba bilježiti na papiru, no elementarno je izmijeniti kod tako da ispisuje ploču koristeći metodu print_board koja je već napisana baš u tu svrhu. 

Za sada je u ovom repositoryu samo kod za model (AI) koji igra igru objektno-orijentirano implementiran u pythonu. U budućnosti planiram zbog brzine dodati implementaciju u C++-u i korisničko sučelje na kojem bi se igra igrala, no za sada se mora igrati na papiru :).
