<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lasagne au radicchio, gorgonzola et noix - Carnet de Recettes</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400&family=Plus+Jakarta+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-color: #FBF9F5;
            --card-bg: #FFFFFF;
            --text-color: #2C2A29;
            --text-muted: #6B6560;
            --accent-color: #A34828;
            --border-color: #E8E2D8;
            --gold-color: #C5A880;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 1.6;
            padding: 2rem 1rem;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
            background-color: var(--card-bg);
            border: 1px solid var(--border-color);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.03);
            border-radius: 12px;
            overflow: hidden;
            padding: 3rem 2.5rem;
        }

        header {
            text-align: center;
            border-bottom: 1px solid var(--border-color);
            padding-bottom: 2.5rem;
            margin-bottom: 2.5rem;
        }

        .subtitle-top {
            font-size: 0.9rem;
            text-transform: uppercase;
            letter-spacing: 3px;
            color: var(--text-muted);
            margin-bottom: 0.5rem;
        }

        h1 {
            font-family: 'Playfair Display', serif;
            font-size: 3rem;
            font-weight: 700;
            color: var(--text-color);
            line-height: 1.2;
            margin-bottom: 0.75rem;
        }

        .tagline {
            font-family: 'Playfair Display', serif;
            font-style: italic;
            color: var(--accent-color);
            font-size: 1.25rem;
        }

        .recipe-meta {
            display: flex;
            justify-content: space-around;
            background-color: var(--bg-color);
            border: 1px solid var(--border-color);
            border-radius: 8px;
            padding: 1.25rem;
            margin-bottom: 3rem;
            text-align: center;
        }

        .meta-item {
            flex: 1;
            border-right: 1px solid var(--border-color);
        }

        .meta-item:last-child {
            border-right: none;
        }

        .meta-label {
            font-size: 0.8rem;
            text-transform: uppercase;
            letter-spacing: 1.5px;
            color: var(--text-muted);
            margin-bottom: 0.25rem;
        }

        .meta-value {
            font-family: 'Playfair Display', serif;
            font-size: 1.15rem;
            font-weight: 600;
        }

        section {
            margin-bottom: 3rem;
        }

        h2 {
            font-family: 'Playfair Display', serif;
            font-size: 2rem;
            margin-bottom: 1.5rem;
            color: var(--text-color);
            border-bottom: 2px solid var(--accent-color);
            display: inline-block;
            padding-bottom: 0.25rem;
        }

        .ingredients-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1.25rem;
        }

        .ingredient-card {
            background-color: var(--bg-color);
            border: 1px solid var(--border-color);
            padding: 1rem;
            border-radius: 8px;
            font-size: 0.95rem;
        }

        .ingredient-card strong {
            display: block;
            font-family: 'Playfair Display', serif;
            font-size: 1.05rem;
            margin-bottom: 0.2rem;
        }

        .step-list {
            list-style: none;
        }

        .step-item {
            display: flex;
            gap: 1.5rem;
            margin-bottom: 1.75rem;
            padding-bottom: 1.75rem;
            border-bottom: 1px dashed var(--border-color);
        }

        .step-item:last-child {
            border-bottom: none;
            margin-bottom: 0;
            padding-bottom: 0;
        }

        .step-number {
            font-family: 'Playfair Display', serif;
            font-size: 2rem;
            font-weight: 700;
            color: var(--accent-color);
            line-height: 1;
            min-width: 40px;
        }

        .step-content h3 {
            font-family: 'Playfair Display', serif;
            font-size: 1.25rem;
            margin-bottom: 0.4rem;
        }

        .step-content p {
            color: var(--text-muted);
            font-size: 0.95rem;
        }

        .tip-box {
            background-color: #FDF8F2;
            border-left: 4px solid var(--accent-color);
            padding: 1.25rem 1.5rem;
            border-radius: 0 8px 8px 0;
            margin-bottom: 2.5rem;
        }

        .tip-box h4 {
            font-family: 'Playfair Display', serif;
            margin-bottom: 0.3rem;
            color: var(--accent-color);
        }

        .tip-box p {
            font-size: 0.95rem;
            color: var(--text-muted);
        }

        .two-cols {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 2rem;
            margin-top: 3rem;
            padding-top: 2rem;
            border-top: 1px solid var(--border-color);
        }

        .info-block h3 {
            font-family: 'Playfair Display', serif;
            font-size: 1.3rem;
            margin-bottom: 1rem;
            color: var(--text-color);
        }

        .info-block ul {
            list-style-type: disc;
            padding-left: 1.25rem;
            color: var(--text-muted);
            font-size: 0.95rem;
        }

        .info-block ul li {
            margin-bottom: 0.5rem;
        }

        .info-block p {
            color: var(--text-muted);
            font-size: 0.95rem;
            margin-bottom: 0.75rem;
        }

        footer {
            text-align: center;
            margin-top: 4rem;
            padding-top: 1.5rem;
            border-top: 1px solid var(--border-color);
            font-size: 0.85rem;
            color: var(--text-muted);
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        @media (max-width: 768px) {
            .container {
                padding: 1.5rem 1rem;
            }
            h1 {
                font-size: 2.2rem;
            }
            .recipe-meta {
                flex-direction: column;
                gap: 1rem;
            }
            .meta-item {
                border-right: none;
                border-bottom: 1px solid var(--border-color);
                padding-bottom: 0.75rem;
            }
            .meta-item:last-child {
                border-bottom: none;
                padding-bottom: 0;
            }
            .two-cols {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>

    <div class="container">
        <header>
            <div class="subtitle-top">Italie &bull; Gourmandise Italienne</div>
            <h1>Lasagne Radicchio</h1>
            <div class="tagline">Saveurs d'automne vénitiennes</div>
        </header>

        <div class="recipe-meta">
            <div class="meta-item">
                <div class="meta-label">Personnes</div>
                <div class="meta-value">4 personnes</div>
            </div>
            <div class="meta-item">
                <div class="meta-label">Préparation</div>
                <div class="meta-value">45 min</div>
            </div>
            <div class="meta-item">
                <div class="meta-label">Cuisson</div>
                <div class="meta-value">40 min <span style="font-size:0.85rem; font-weight:normal; color:var(--text-muted);">(dont 10 min gratin)</span></div>
            </div>
            <div class="meta-item">
                <div class="meta-label">Difficulté</div>
                <div class="meta-value">Intermédiaire</div>
            </div>
        </div>

        <section>
            <h2>Ingrédients</h2>
            <div class="ingredients-grid">
                <div class="ingredient-card">
                    <strong>Radicchio tardif</strong> 2 têtes
                </div>
                <div class="ingredient-card">
                    <strong>Pâtes à lasagne</strong> Fraîches
                </div>
                <div class="ingredient-card">
                    <strong>Gorgonzola</strong> Crémeux
                </div>
                <div class="ingredient-card">
                    <strong>Noix décortiquées</strong> 100 g
                </div>
                <div class="ingredient-card">
                    <strong>Lait entier</strong> 750 ml
                </div>
                <div class="ingredient-card">
                    <strong>Beurre</strong> 60 g
                </div>
                <div class="ingredient-card">
                    <strong>Farine de blé</strong> 60 g
                </div>
                <div class="ingredient-card">
                    <strong>Parmesan râpé</strong> 80 g
                </div>
                <div class="ingredient-card">
                    <strong>Échalote</strong> 1
                </div>
                <div class="ingredient-card">
                    <strong>Safran</strong> 1 pincée
                </div>
            </div>
        </section>

        <div class="tip-box">
            <h4>Astuce du chef</h4>
            <p>Pour un radicchio moins amer, faites-le revenir brièvement avec de l'échalote avant de l'ajouter à la béchamel. Le radicchio doit être saisi rapidement pour conserver sa couleur vive et sa texture.</p>
        </div>

        <section>
            <h2>Préparation</h2>
            <ul class="step-list">
                <li class="step-item">
                    <div class="step-number">1</div>
                    <div class="step-content">
                        <h3>Préparer le radicchio</h3>
                        <p>Lavez le radicchio, essuyez-le et coupez-le en fines lanières. Émincez l'échalote.</p>
                    </div>
                </li>
                <li class="step-item">
                    <div class="step-number">2</div>
                    <div class="step-content">
                        <h3>Cuire le radicchio</h3>
                        <p>Dans une poêle avec un peu d'huile, faites suer l'échalote, puis ajoutez le radicchio et faites-le fondre 5-7 min. Salez, poivrez.</p>
                    </div>
                </li>
                <li class="step-item">
                    <div class="step-number">3</div>
                    <div class="step-content">
                        <h3>Préparer la béchamel</h3>
                        <p>Fondez le beurre, ajoutez la farine, puis versez le lait chaud petit à petit en remuant jusqu'à épaississement. Salez, poivrez, muscadez. <em>(Pour une béchamel sans grumeaux, veillez à ce que le mélange beurre/farine soit bien cuit — roux blanc — avant d'ajouter le lait).</em></p>
                    </div>
                </li>
                <li class="step-item">
                    <div class="step-number">4</div>
                    <div class="step-content">
                        <h3>Mélanger</h3>
                        <p>Ajoutez la moitié du gorgonzola en dés dans la béchamel chaude et remuez jusqu'à ce qu'il fonde. Incorporez le radicchio.</p>
                    </div>
                </li>
                <li class="step-item">
                    <div class="step-number">5</div>
                    <div class="step-content">
                        <h3>Monter les lasagnes</h3>
                        <p>Dans un plat beurré, alternez pâte, béchamel au radicchio, parmesan et noix concassées. Répétez l'opération.</p>
                    </div>
                </li>
                <li class="step-item">
                    <div class="step-number">6</div>
                    <div class="step-content">
                        <h3>Terminer</h3>
                        <p>Recouvrez la dernière couche de pâtes avec le reste de béchamel, parsemez le reste de gorgonzola et de parmesan.</p>
                    </div>
                </li>
                <li class="step-item">
                    <div class="step-number">7</div>
                    <div class="step-content">
                        <h3>Cuire</h3>
                        <p>Enfournez à 180°C pendant 30 min de cuisson, puis 10 min sous le grill pour gratiner. Laissez reposer 10 min.</p>
                    </div>
                </li>
            </ul>
        </section>

        <div class="two-cols">
            <div class="info-block">
                <h3>Accords & Saveurs</h3>
                <p><strong>Côté vins :</strong></p>
                <ul>
                    <li>Un vin rouge charpenté type Valpolicella.</li>
                    <li>Un vin blanc sec et minéral.</li>
                </ul>
                <p style="margin-top: 1rem;"><strong>Côté autres accompagnements :</strong></p>
                <ul>
                    <li>Une salade de roquette et vinaigre balsamique.</li>
                    <li>Un vin de dessert italien type Vin Santo.</li>
                    <li>Une grappa en digestif.</li>
                </ul>
            </div>
            
            <div class="info-block">
                <h3>Une histoire de terroir</h3>
                <p>La lasagne est un plat de pâtes emblématique d'Émilie-Romagne, mais cette version automnale est inspirée de la tradition vénitienne, mettant à l'honneur le radicchio.</p>
                <p>Le radicchio di Treviso, avec son amertume délicate, équilibre parfaitement la richesse du gorgonzola et le croquant des noix, créant une symphonie de saveurs.</p>
            </div>
        </div>

        <footer>
            Carnet de Recettes &bull; Un plat généreux à partager en famille ou entre amis
        </footer>
    </div>

</body>
</html>