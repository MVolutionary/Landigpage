<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mehr Firmen-Leads – Lokaler AI-Webseiten-Service mit Google & Meta Ads</title>
    <meta name="description" content="Mehr Kundenanfragen für Ihr Unternehmen durch maßgeschneiderte AI-Landingpages und gezielte Werbeanzeigen. Lokaler Dienstleister für Lead-Generierung.">
    <link href="https://fonts.googleapis.com/css?family=Montserrat:400,700&display=swap" rel="stylesheet">
    <style>
        :root {
            --gold: #d4af37;
            --dark: #161616;
            --darker: #101010;
            --white: #f7f7f7;
            --text-light: #e5e5e5;
            --grey: #292929;
        }

        html, body {
            margin: 0;
            padding: 0;
            background: var(--dark);
            color: var(--white);
            font-family: 'Montserrat', Arial, sans-serif;
            scroll-behavior: smooth;
        }

        .hero {
            min-height: 100vh;
            background: linear-gradient(120deg, #101010 60%, #232323 100%);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: center;
            position: relative;
        }
        .hero h1 {
            font-size: 2.5rem;
            font-weight: 700;
            background: linear-gradient(90deg, var(--gold), #fffbe6 90%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: goldmove 2.5s linear infinite alternate;
            letter-spacing: 0.02em;
            margin-bottom: 1rem;
        }
        @keyframes goldmove {
            0% {background-position: 0%;}
            100% {background-position: 100%;}
        }
        .hero p {
            font-size: 1.23rem;
            color: var(--text-light);
            margin-bottom: 2.2rem;
            max-width: 560px;
            margin-left: auto;
            margin-right: auto;
        }
        .hero .cta-btn {
            background: linear-gradient(90deg, var(--gold) 30%, #fffbe6 100%);
            color: var(--dark);
            font-weight: bold;
            font-size: 1.2rem;
            padding: 1.1rem 2.9rem;
            border: none;
            border-radius: 40px;
            cursor: pointer;
            text-decoration: none;
            box-shadow: 0 4px 20px 0 #d4af3733, 0 0 24px #d4af37aa;
            transition: background .25s, transform .2s;
        }
        .hero .cta-btn:hover {
            background: linear-gradient(90deg, #fffbe6 30%, var(--gold) 100%);
            transform: scale(1.04);
        }
        .hero .down-arrow {
            margin-top: 60px;
            font-size: 2.5rem;
            color: var(--gold);
            animation: bounce 1.5s infinite;
        }
        @keyframes bounce {
            0%, 100% { transform: translateY(0);}
            50% { transform: translateY(14px);}
        }
        section {
            max-width: 950px;
            margin: 3.5rem auto 3rem auto;
            background: var(--darker);
            border-radius: 18px;
            padding: 2.5rem 2.2rem;
            box-shadow: 0 8px 38px 0 rgba(0,0,0,0.11);
        }
        section h2 {
            color: var(--gold);
            font-size: 2.1rem;
            font-weight: 700;
            margin-bottom: 1.4rem;
            letter-spacing: 0.01em;
        }
        .features-list {
            display: flex;
            flex-wrap: wrap;
            gap: 2.5rem 2rem;
            margin-top: 2rem;
        }
        .feature {
            flex: 1 1 260px;
            background: #232323;
            border-radius: 12px;
            padding: 1.5rem 1.2rem 1.2rem 1.7rem;
            margin-bottom: 1rem;
            min-width: 220px;
            box-shadow: 0 2px 12px 0 #d4af3733;
            position: relative;
            border-left: 5px solid var(--gold);
        }
        .feature-title {
            color: var(--gold);
            font-size: 1.18rem;
            font-weight: 600;
            margin-bottom: 0.7rem;
        }
        .feature-desc {
            color: var(--white);
            opacity: 0.96;
            font-size: 1.04rem;
        }

        /* Preis-Pakete */
        .pakete-section {
            background: linear-gradient(120deg, #181818 85%, #232323 100%);
            border-radius: 22px;
            box-shadow: 0 8px 38px 0 rgba(212,175,55,0.10), 0 1.5px 6px 0 #d4af3722;
            padding: 2.7rem 1.2rem 2.6rem 1.2rem;
            max-width: 950px;
            margin: 3rem auto 3rem auto;
        }
        .pakete-overview {
            display: flex;
            justify-content: space-around;
            gap: 2.5rem;
            flex-wrap: wrap;
            margin-top: 1.2rem;
        }
        .paket {
            background: #232323;
            border: 2.5px solid #d4af37;
            border-radius: 18px;
            box-shadow: 0 4px 30px 0 #d4af3730;
            padding: 2.2rem 1.2rem 2.4rem 1.2rem;
            flex: 1 1 260px;
            min-width: 220px;
            max-width: 330px;
            margin-bottom: 1.7rem;
            display: flex;
            flex-direction: column;
            align-items: center;
            transition: transform .20s, box-shadow .20s;
        }
        .paket:hover {
            transform: scale(1.04);
            box-shadow: 0 12px 44px 0 #d4af3733, 0 0 24px #d4af3733;
            z-index: 2;
        }
        .paket-title {
            font-size: 1.3rem;
            font-weight: 700;
            color: #fffbe6;
            margin-bottom: 0.5rem;
            letter-spacing: 0.02em;
        }
        .paket-preis {
            font-size: 2.0rem;
            font-weight: 800;
            color: var(--gold);
            margin-bottom: 1.2rem;
            letter-spacing: 0.03em;
        }
        .paket-vorteile {
            color: #fffbe6;
            font-size: 1.04rem;
            margin-bottom: 2.1rem;
            text-align: left;
        }
        .paket-vorteile li {
            margin-bottom: 0.6rem;
            position: relative;
            padding-left: 1.3em;
        }
        .paket-vorteile li:before {
            content: "✓";
            color: var(--gold);
            font-size: 1.15em;
            left: 0;
            position: absolute;
        }
        .paket-btn {
            background: linear-gradient(90deg, #d4af37 30%, #fffbe6 100%);
            color: #161616;
            font-weight: 700;
            font-size: 1.09rem;
            padding: 0.8rem 2.1rem;
            border: none;
            border-radius: 40px;
            cursor: pointer;
            box-shadow: 0 4px 20px 0 #d4af3731;
            transition: background .23s, transform .18s;
            margin-top: 1rem;
            text-decoration: none;
        }
        .paket-btn:hover {
            background: linear-gradient(90deg, #fffbe6 24%, #d4af37 100%);
            transform: scale(1.06);
        }

        .demo-section {
            text-align: center;
            background: linear-gradient(110deg, #181818 70%, #232323 100%);
            margin-top: 3.5rem;
        }
        .demo-img {
            display: block;
            margin: 2.2rem auto 0 auto;
            width: 93%;
            max-width: 430px;
            border-radius: 12px;
            border: 2.5px solid var(--gold);
            box-shadow: 0 10px 28px 0 #d4af3715, 0 0 24px #d4af37aa;
            transition: transform 0.3s;
        }
        .demo-img:hover {
            transform: scale(1.03) rotate(-1deg);
            box-shadow: 0 16px 44px 0 #d4af3720;
        }
        .steps {
            display: flex;
            flex-direction: column;
            gap: 1.45rem;
            margin-top: 2.3rem;
        }
        .step {
            background: var(--grey);
            border-left: 5px solid var(--gold);
            padding: 1.4rem 1.7rem;
            border-radius: 12px;
            font-size: 1.08rem;
            box-shadow: 0 2px 14px 0 #d4af3720;
            color: var(--text-light);
        }
        .step span {
            font-weight: bold;
            color: var(--gold);
            font-size: 1.15rem;
            margin-right: 0.7em;
        }

        .testimonial {
            font-style: italic;
            background: rgba(255,255,255,0.04);
            border-left: 4px solid var(--gold);
            padding: 1.4rem 1.5rem;
            border-radius: 12px;
            margin-bottom: 1.2rem;
            color: #f0e6cc;
            box-shadow: 0 1px 8px 0 #d4af3720;
            transition: box-shadow 0.2s;
        }
        .testimonial:hover {
            box-shadow: 0 6px 24px 0 #d4af3720, 0 0 24px #d4af3733;
        }

        #kontakt {
            background: linear-gradient(120deg, #181818 85%, #232323 100%);
            border-radius: 22px;
            box-shadow: 0 8px 38px 0 rgba(212,175,55,0.10), 0 1.5px 6px 0 #d4af3722;
            padding: 2.5rem 2.2rem 2.7rem 2.2rem;
            max-width: 520px;
            margin: 3.5rem auto 3rem auto;
        }
        #kontakt h2 {
            color: #d4af37;
            font-size: 2rem;
            font-weight: 700;
            margin-bottom: 2.1rem;
            text-align: center;
            letter-spacing: 0.01em;
        }
        #form-container {
            margin-bottom: 0.5rem;
        }
        #fancy-contact-form {
            display: flex;
            flex-direction: column;
            gap: 1.7rem;
        }
        .form-group {
            position: relative;
            margin-bottom: 8px;
        }
        .form-group input,
        .form-group textarea {
            width: 100%;
            border: none;
            border-bottom: 2.5px solid #444;
            background: transparent;
            color: #f7f7f7;
            font-size: 1.16rem;
            padding: 1.1rem 0 0.6rem 0.2rem;
            outline: none;
            transition: border-color .22s, box-shadow .22s;
            box-shadow: none;
            border-radius: 0;
            font-family: 'Montserrat', Arial, sans-serif;
        }
        .form-group input[type="file"] {
            color: #d4af37;
            background: none;
            border: none;
            padding: 0;
            font-size: 1rem;
        }
        .form-group label {
            position: absolute;
            left: 0.2rem;
            top: 1.25rem;
            color: #b5b5b5;
            font-size: 1.04rem;
            pointer-events: none;
            transition: all .23s cubic-bezier(.4,0,.2,1);
            letter-spacing: 0.01em;
            background: none;
            padding: 0 0.12em;
            border-radius: 6px;
        }
        .form-group input:focus,
        .form-group textarea:focus {
            border-color: #d4af37;
            box-shadow: 0 2px 16px 0 #d4af3740;
        }
        .form-group input:focus ~ label,
        .form-group input:not(:placeholder-shown):not([type="file"]) ~ label,
        .form-group textarea:focus ~ label,
        .form-group textarea:not(:placeholder-shown) ~ label {
            top: -0.7rem;
            left: 0;
            font-size: 0.93rem;
            color: #d4af37;
            background: #181818;
            padding: 0 0.3em;
            box-shadow: 0 2px 10px 0 #d4af3715;
        }
        .form-group input[type="file"] ~ label.file-label {
            position: static;
            color: #d4af37;
            font-size: 1.02rem;
            opacity: 0.83;
            margin-top: 0.2rem;
            margin-bottom: 0.1rem;
            left: auto;
            top: auto;
            background: none;
            padding: 0;
        }
        .fancy-btn {
            background: linear-gradient(90deg, #d4af37 40%, #fffbe6 100%);
            color: #161616;
            font-weight: 700;
            font-size: 1.13rem;
            padding: 1rem 2.1rem;
            border: none;
            border-radius: 40px;
            cursor: pointer;
            box-shadow: 0 4px 20px 0 #d4af3731, 0 0 18px #d4af3717;
            transition: background .23s, transform .18s, box-shadow .18s;
            margin-top: 0.6rem;
            letter-spacing: 0.01em;
        }
        .fancy-btn:hover {
            background: linear-gradient(90deg, #fffbe6 24%, #d4af37 100%);
            transform: scale(1.04);
            box-shadow: 0 8px 32px 0 #d4af3737, 0 0 24px #d4af3737;
        }
        .whatsapp-btn {
            display: inline-block;
            margin-top: 2.5rem;
            padding: 0.8rem 2rem;
            background: none;
            color: #d4af37;
            border: 2px solid #d4af37;
            border-radius: 40px;
            font-weight: 600;
            font-size: 1.08rem;
            text-decoration: none;
            box-shadow: 0 2px 8px 0 #d4af3715;
            transition: background .15s, color .15s, transform .15s;
        }
        .whatsapp-btn:hover {
            background: #d4af37;
            color: #161616;
            transform: scale(1.04);
        }
        #form-success {
            background: linear-gradient(90deg, #232323 70%, #181818 100%);
            border: 2px solid #d4af37;
            border-radius: 20px;
            color: #fffbe6;
            text-align: center;
            font-size: 1.25rem;
            font-weight: 600;
            padding: 2.4rem 1.1rem;
            margin-top: 1.6rem;
            box-shadow: 0 2px 18px 0 #d4af3723;
            animation: popsuccess 0.8s cubic-bezier(.2,1.2,.6,1);
        }
        @keyframes popsuccess {
            0% { opacity: 0; transform: scale(0.7);}
            80% { transform: scale(1.1);}
            100% { opacity: 1; transform: scale(1);}
        }
        @media (max-width: 1100px) {
            .pakete-overview { flex-direction: column; align-items: center; }
            .paket { max-width: 480px; width: 90%; }
        }
        @media (max-width: 900px) {
            section, .pakete-section { padding: 1.7rem 0.7rem; }
            .features-list { flex-direction: column; gap: 1.3rem; }
        }
        @media (max-width: 700px) {
            #kontakt, .pakete-section { padding: 1.2rem 0.4rem 1.7rem 0.4rem; }
            #kontakt h2 { font-size: 1.2rem;}
        }
        @media (max-width: 600px) {
            .hero h1 { font-size: 2.1rem; }
            section h2 { font-size: 1.2rem; }
            .demo-img { width: 98%; }
            .feature { padding: 1.2rem 0.7rem 1rem 1rem; }
        }
        footer {
            text-align: center;
            padding: 2.4rem 0 1.1rem 0;
            color: #777;
            font-size: 1rem;
            background: #111;
            margin-top: 2.2rem;
            letter-spacing: 0.02em;
        }
    </style>
</head>
<body>
    <!-- Hero Section -->
    <div class="hero">
        <h1>Mehr Firmen-Leads für Ihr Unternehmen</h1>
        <p>
            Lokaler Partner für hochwertige Kundenanfragen:<br>
            AI-generierte Landingpages, zielgerichtete Google- & Meta Ads.<br>
            <span style="color:var(--gold);font-weight:700;">Steigern Sie Ihren Umsatz um bis zu 100 % – mit einer Webseite, die überzeugt und verkauft.</span>
        </p>
        <a href="#pakete" class="cta-btn">Jetzt Angebot sichern</a>
        <div class="down-arrow" title="Scrollen für mehr Info">&#x25BC;</div>
    </div>

    <!-- Was wir machen -->
    <section>
        <h2>Was wir für Sie tun:</h2>
        <div class="features-list">
            <div class="feature">
                <div class="feature-title">AI-Landingpages, die verkaufen</div>
                <div class="feature-desc">
                    Wir erstellen für Sie maßgeschneiderte, KI-optimierte Webseiten, die Besucher automatisch in echte Anfragen und Kunden verwandeln.
                </div>
            </div>
            <div class="feature">
                <div class="feature-title">Leads durch Google & Meta Ads</div>
                <div class="feature-desc">
                    Mit gezielten Werbeanzeigen auf Google und Meta (Facebook/Instagram) werden Ihre Wunschkunden direkt auf Ihre Seite gelenkt.
                </div>
            </div>
            <div class="feature">
                <div class="feature-title">Alles aus einer Hand – lokal und persönlich</div>
                <div class="feature-desc">
                    Wir sind Ihr Ansprechpartner vor Ort, übernehmen Technik, Texte, Design und Vermarktung. Sie konzentrieren sich auf Ihr Geschäft – wir liefern die Anfragen.
                </div>
            </div>
        </div>
    </section>

    <!-- Vorteile -->
    <section>
        <h2>Ihre Vorteile mit uns:</h2>
        <ul style="color:#fffbe6;font-size:1.09rem;line-height:1.7;">
            <li><b>Maximale Sichtbarkeit:</b> Ihre Firma wird genau dort gefunden, wo Ihre Kunden suchen – regional, gezielt und messbar.</li>
            <li><b>Messbare Resultate:</b> Sie erhalten monatlich echte Leads und sehen schwarz auf weiß, wie Ihr Werbebudget arbeitet.</li>
            <li><b>100 % Fokus auf Neukundengewinnung:</b> Jede Seite und jede Anzeige ist darauf ausgelegt, Interessenten in zahlende Kunden zu wandeln.</li>
            <li><b>Deutliche Umsatzsteigerung:</b> Mit einer überzeugenden Online-Präsenz, die Vertrauen schafft, können Sie Ihre Auftragslage und Ihren Umsatz verdoppeln.</li>
            <li><b>Kundenzufriedenheit:</b> Unsere Kunden berichten von mehr Anfragen, besseren Kunden und spürbarem Wachstum.</li>
        </ul>
    </section>

    <!-- Preis-Pakete -->
    <section class="pakete-section" id="pakete">
        <h2>Wählen Sie Ihr Erfolgs-Paket:</h2>
        <div class="pakete-overview">
            <div class="paket">
                <div class="paket-title">Starter-Paket</div>
                <div class="paket-preis">1.500&nbsp;€</div>
                <ul class="paket-vorteile">
                    <li>AI-Landingpage inkl. Design und Text</li>
                    <li>Optimiert für Google-Sichtbarkeit</li>
                    <li>Grundlegende Conversion-Optimierung</li>
                    <li>1-wöchige Betreuung</li>
                </ul>
                <a href="#kontakt" class="paket-btn">Anfragen</a>
            </div>
            <div class="paket" style="border-width:3.5px;box-shadow:0 8px 36px 0 #d4af3770;">
                <div class="paket-title">Business-Paket</div>
                <div class="paket-preis">2.800&nbsp;€</div>
                <ul class="paket-vorteile">
                    <li>AI-Landingpage inkl. Logo & individuelle Inhalte</li>
                    <li>Google & Meta (Facebook/Instagram) Ads Einrichtung</li>
                    <li>Conversion-Tracking & Analytics</li>
                    <li>1 Monat Betreuung & Optimierung</li>
                </ul>
                <a href="#kontakt" class="paket-btn">Anfragen</a>
            </div>
            <div class="paket">
                <div class="paket-title">Premium-Paket</div>
                <div class="paket-preis">4.500&nbsp;€</div>
                <ul class="paket-vorteile">
                    <li>Komplette AI-Webseite mit mehreren Landingpages</li>
                    <li>Google & Meta Ads Kampagnen inkl. laufender Optimierung</li>
                    <li>Lead-Management & CRM-Anbindung</li>
                    <li>3 Monate persönliche Betreuung</li>
                </ul>
                <a href="#kontakt" class="paket-btn">Anfragen</a>
            </div>
        </div>
        <div style="text-align:center;color:#fffbe6;font-size:1.08rem;margin-top:1.5rem;">
            <em>Sie wissen nicht, welches Paket passt? Schreiben Sie uns – wir beraten Sie ehrlich und persönlich!</em>
        </div>
    </section>

    <!-- Demo -->
    <section class="demo-section">
        <h2>So kann Ihre neue Landingpage aussehen:</h2>
        <img src="https://dummyimage.com/900x500/232323/d4af37&text=AI+Landingpage+Demo" alt="Webseiten Demo" class="demo-img">
        