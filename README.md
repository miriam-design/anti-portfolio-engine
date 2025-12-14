TOTEM Engine 🗿

"Non è un sito web. È un monumento digitale alla tua identità."

Questa è la Rendering Engine standalone del progetto TOTEM (Anti-Portfolio).
È un visualizzatore 3D ad alte prestazioni costruito con Next.js, Three.js e React Three Fiber.
Il suo unico scopo è prendere un file di configurazione (dna.json) generato dall'AI e renderizzare un'esperienza 3D interattiva, unica per ogni persona.

🚀 Come Funziona
L'ecosistema TOTEM è diviso in due parti:
The Forge (Generator): Il tool AI che ti intervista e crea il tuo "DNA Digitale".
The Engine (Questa Repo): Il visualizzatore che legge quel DNA e lo trasforma in realtà.Tu sei qui. Questa è la "Console". Hai bisogno della "Cartuccia" (dna.json) per farla funzionare.

🛠️ Installazione Locale
Clona la repository:git clone [https://github.com/miriam-design/anti-portfolio-engine.git](https://github.com/miriam-design/anti-portfolio-engine.git)
cd anti-portfolio-engine
Installa le dipendenze:npm install
(Nota: Questo scaricherà React, Three.js e tutto il necessario nella cartella node_modules locale).

Inserisci il tuo DNA:Prendi il file dna.json che hai scaricato dal Generator Tool.
Spostalo dentro la cartella public/ di questo progetto.
Attenzione: Se esiste già un file con quel nome, sovrascrivilo.
Avvia l'Engine:npm run dev
Apri http://localhost:3000 per vedere il tuo Totem prendere vita.

🌍 Come Pubblicare Online (Gratis)
Puoi mettere online il tuo Anti-Portfolio in meno di 2 minuti usando Vercel.
Fai un Fork di questa repository sul tuo account GitHub.
Carica il tuo DNA:
Vai sulla tua repo forkata su GitHub.
Naviga nella cartella public/.
Clicca su "Add file" -> "Upload files".
Carica il tuo dna.json personale.
Clicca "Commit changes".
Deploy:Vai su Vercel.com e accedi.
Clicca "Add New Project".
Importa la tua repository GitHub.
Clicca Deploy.Fatto. Il tuo Totem è online e accessibile a tutto il mondo.

🎨 Personalizzazione AvanzataAnche se l'AI decide lo stile visivo, tu hai il controllo completo del codice.
Struttura del file dna.jsonL'engine si aspetta un file JSON con questa struttura specifica per il visual_dna:
"visual_dna": {
  "geometry_type": "sphere" | "torus" | "cluster" | "pyramid" ...,
  "material_type": "glass" | "wireframe" | "metal" | "stone" ...,
  "movement_speed": "slow" | "fast",
  "colors": {
    "bg": "#1a1a1a",     // Colore di sfondo
    "primary": "#ff00ff", // Colore principale del Totem
    "secondary": "#00ffff" // Colore dei dettagli/luci
  }
}
Puoi modificare manualmente questi valori nel file JSON per cambiare radicalmente l'aspetto del tuo sito senza toccare il codice React.

📦 Tech StackFramework: Next.js 14 (App Router)
Styling: Tailwind CSS
3D Engine: React Three Fiber (@react-three/fiber)
3D Helpers: Drei (@react-three/drei)Motion: Framer Motion

📄 Licenza
Questo progetto è open source sotto licenza MIT.
Sentiti libero di forkare, hackerare e distruggere questo engine per costruire qualcosa di ancora più strano.Generato dal Protocollo TOTEM.
