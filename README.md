<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>WADDLY Coin - The Future Meme Coin on Solana</title>
    <style>
        /* Reset & base */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        body {
            background: linear-gradient(135deg, #141727, #1b2238);
            color: #f0f0f0;
            line-height: 1.6;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
        }
        a {
            color: #4ef3e6;
            text-decoration: none;
        }
        a:hover {
            text-decoration: underline;
        }
        header {
            background: #0e141f;
            padding: 1rem 2rem;
            display: flex;
            align-items: center;
            justify-content: space-between;
            border-bottom: 1px solid #2d3555;
        }
        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            color: #4ef3e6;
            display: flex;
            align-items: center;
        }
        .logo img {
            width: 48px;
            height: 48px;
            margin-right: 12px;
        }
        nav ul {
            list-style: none;
            display: flex;
            gap: 1.5rem;
        }
        nav ul li a {
            font-weight: 600;
            font-size: 1rem;
            padding: 0.3rem 0.5rem;
            transition: background-color 0.3s ease;
            border-radius: 4px;
        }
        nav ul li a:hover {
            background: #4ef3e6;
            color: #0e141f;
        }
        main {
            flex-grow: 1;
            max-width: 1200px;
            margin: 2rem auto 4rem auto;
            padding: 0 1rem;
        }
        .hero {
            text-align: center;
            margin-bottom: 3rem;
        }
        .hero h1 {
            font-size: 2.5rem;
            color: #4ef3e6;
            margin-bottom: 1rem;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 0.6rem;
        }
        .hero h1 .penguin {
            width: 40px;
            height: 40px;
            display: inline-block;
            background: url('https://cdn-icons-png.flaticon.com/512/616/616408.png') no-repeat center/contain;
        }
        .hero p {
            font-size: 1.2rem;
            color: #d0f7f3;
            margin-bottom: 1.8rem;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }
        .btn-group {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
        }
        .btn {
            padding: 0.75rem 1.8rem;
            font-size: 1rem;
            font-weight: 600;
            border-radius: 40px;
            border: none;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            color: #0e141f;
            background: #4ef3e6;
            box-shadow: 0 4px 15px rgba(78, 243, 230, 0.6);
        }
        .btn:hover {
            background: #36c4be;
            box-shadow: 0 6px 20px rgba(54, 196, 190, 0.8);
        }
        section {
            margin-bottom: 3rem;
            background: #1f2842;
            padding: 2rem 2rem;
            border-radius: 12px;
            box-shadow: 0 0 30px #0ef3e6aa;
        }
        section h2 {
            color: #4ef3e6;
            font-size: 2rem;
            margin-bottom: 1.5rem;
            text-align: center;
        }
        .tokenomics-list, .roadmap-list, .why-list, .social-list {
            max-width: 700px;
            margin: 0 auto;
            list-style: none;
            padding-left: 0;
            font-size: 1.1rem;
            color: #b5f7f3;
        }
        .tokenomics-list li, .roadmap-list li, .why-list li, .social-list li {
            margin-bottom: 0.9rem;
            padding-left: 1.5rem;
            position: relative;
        }
        .tokenomics-list li::before, .roadmap-list li::before, .why-list li::before {
            content: '•';
            position: absolute;
            left: 0;
            color: #4ef3e6;
            font-weight: bold;
            font-size: 1.4rem;
            line-height: 1rem;
        }
        .roadmap-list li {
            margin-bottom: 2rem;
        }
        .roadmap-list li strong {
            display: block;
            font-weight: 700;
            font-size: 1.2rem;
            margin-bottom: 0.4rem;
            color: #81e1de;
        }
        footer {
            background: #0a0f18;
            padding: 1.5rem 2rem;
            text-align: center;
            font-size: 0.9rem;
            color: #3fdde4;
            box-shadow: inset 0 2px 6px #0a0f1866;
        }
        footer a {
            color: #3fdde4;
        }
        footer a:hover {
            text-decoration: underline;
        }
        /* Responsive */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 1.8rem;
            }
            .btn-group {
                flex-direction: column;
                gap: 1rem;
            }
            nav ul {
                flex-direction: column;
                gap: 1rem;
            }
        }
        /* Community Tools & Games Section */
        #community-tools {
            background: #123456;
            padding: 2rem;
            border-radius: 12px;
            max-width: 700px;
            margin: 0 auto 3rem auto;
            color: #cce7e7;
            box-shadow: 0 0 25px #0ef3e6aa;
        }
        #community-tools h2 {
            margin-bottom: 1rem;
            color: #4ef3e6;
        }
        #community-tools p {
            margin-bottom: 1rem;
            font-size: 1.1rem;
            line-height: 1.4;
        }
        #community-tools a {
            color: #4ef3e6;
            font-weight: bold;
            text-decoration: none;
        }
        #community-tools a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
<header>
    <div class="logo">
        <img src="https://cdn-icons-png.flaticon.com/512/616/616408.png" alt="WADDLY Penguin Logo" />
        WADDLY Coin
    </div>
    <nav>
        <ul>
            <li><a href="#hero">Home</a></li>
            <li><a href="#tokenomics">Tokenomics</a></li>
            <li><a href="#roadmap">Roadmap</a></li>
            <li><a href="#why">Why WADDLY?</a></li>
            <li><a href="#community-tools">Community</a></li>
            <li><a href="#footer">Contact</a></li>
        </ul>
    </nav>
</header>

<main>
    <section id="hero" class="hero">
        <h1>Meet WADDLY <span class="penguin"></span></h1>
        <p>The Meme Coin of the Future, Built on Solana.<br>Moon-bound, duck-powered, and fully community-driven.</p>
        <div class="btn-group">
            <a href="https://t.me/waddlycoin" class="btn" target="_blank" rel="noopener">🚀 Buy WADDLY Now</a>
            <a href="#" class="btn" target="_blank" rel="noopener">📄 View Whitepaper</a>
        </div>
    </section>

    <section id="tokenomics">
        <h2>Tokenomics</h2>
        <ul class="tokenomics-list">
            <li>Total Supply: 100,000,000,000 WADDLY</li>
            <li>Network: Solana</li>
            <li>50% — Community Rewards</li>
            <li>20% — Liquidity & CEX Listings</li>
            <li>15% — Marketing & Partnerships</li>
            <li>10% — Team (1 Year Lock)</li>
            <li>5% — Burn Mechanism</li>
        </ul>
    </section>

    <section id="roadmap">
        <h2>Roadmap</h2>
        <ul class="roadmap-list">
            <li><strong>Q1 2026</strong> — Launch of WADDLY, Website & Whitepaper v1, Initial Airdrop Campaign</li>
            <li><strong>Q2 2026</strong> — CoinMarketCap & CoinGecko Listing, 10K+ Holders, First NFT Teasers</li>
            <li><strong>Q3 2026</strong> — Major CEX Listing, Meme Contest, Community DAO Voting</li>
            <li><strong>Q4 2026</strong> — NFT Collection Launch, P2E Game Sneak Peek, Token Burn Event</li>
        </ul>
    </section>

    <section id="why">
        <h2>Why WADDLY?</h2>
        <ul class="why-list">
            <li>Built on blazing-fast Solana</li>
            <li>Meme-fueled, community-powered</li>
            <li>Transparent, fair launch – no VC games</li>
            <li>NFTs, P2E game, staking & more coming</li>
        </ul>
    </section>

    <section id="community-tools">
        <h2>Community Tools & Games</h2>
        <p>Our Telegram bot lets you stay updated with the latest WADDLY news, participate in quizzes, play games, and even earn rewards — all inside Telegram!</p>
        <p>Get ready for upcoming mini-games and challenges that bring fun and rewards together for the WADDLY community.</p>
        <a href="https://t.me/waddlycoin" target="_blank" rel="noopener">Join our Telegram Bot & Community →</a>
    </section>
</main>

<footer id="footer">
    <p>Join our community:</p>
    <ul class="social-list">
        <li><a href="https://t.me/waddlycoin" target="_blank" rel="noopener">Telegram</a></li>
        <li><a href="https://twitter.com/waddlysol" target="_blank" rel="noopener">Twitter</a></li>
        <li><a href="#" target="_blank" rel="noopener">Whitepaper (coming soon)</a></li>
    </ul>
    <p>&copy; 2025 WADDLY Coin. All rights reserved.</p>
</footer>
</body>
</html>
