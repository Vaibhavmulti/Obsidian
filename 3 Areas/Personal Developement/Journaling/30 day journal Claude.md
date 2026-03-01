
file:///Users/vaibhav/Downloads/30-day-journal-plan.html







<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Your 30-Day Journal Journey</title>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300;1,400&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --cream: #faf6f0;
    --warm: #f2ebe0;
    --sand: #e8dece;
    --clay: #c4956a;
    --earth: #8b6347;
    --bark: #4a3728;
    --sage: #7a9e7e;
    --blush: #d4917a;
    --ink: #2c1f14;
    --muted: #8a7567;
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }

  body {
    background-color: var(--cream);
    color: var(--ink);
    font-family: 'DM Sans', sans-serif;
    font-weight: 300;
    line-height: 1.7;
    min-height: 100vh;
  }

  /* Texture overlay */
  body::before {
    content: '';
    position: fixed;
    inset: 0;
    background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.04'/%3E%3C/svg%3E");
    pointer-events: none;
    z-index: 0;
  }

  .page {
    max-width: 860px;
    margin: 0 auto;
    padding: 60px 40px;
    position: relative;
    z-index: 1;
  }

  /* Header */
  header {
    text-align: center;
    margin-bottom: 80px;
    padding-bottom: 60px;
    border-bottom: 1px solid var(--sand);
    position: relative;
  }

  header::after {
    content: '✦';
    position: absolute;
    bottom: -14px;
    left: 50%;
    transform: translateX(-50%);
    background: var(--cream);
    padding: 0 16px;
    color: var(--clay);
    font-size: 18px;
  }

  .subtitle {
    font-family: 'DM Sans', sans-serif;
    font-size: 11px;
    letter-spacing: 0.25em;
    text-transform: uppercase;
    color: var(--clay);
    margin-bottom: 24px;
  }

  h1 {
    font-family: 'Cormorant Garamond', serif;
    font-size: clamp(2.8rem, 5vw, 4.2rem);
    font-weight: 300;
    line-height: 1.15;
    color: var(--bark);
    margin-bottom: 20px;
  }

  h1 em {
    font-style: italic;
    color: var(--clay);
  }

  .intro-text {
    font-size: 15px;
    color: var(--muted);
    max-width: 520px;
    margin: 0 auto 32px;
  }

  .tags {
    display: flex;
    gap: 10px;
    justify-content: center;
    flex-wrap: wrap;
  }

  .tag {
    padding: 6px 18px;
    border-radius: 100px;
    font-size: 12px;
    letter-spacing: 0.05em;
    border: 1px solid;
  }

  .tag-identity { border-color: var(--clay); color: var(--clay); background: rgba(196, 149, 106, 0.08); }
  .tag-growth { border-color: var(--sage); color: var(--sage); background: rgba(122, 158, 126, 0.08); }
  .tag-relationships { border-color: var(--blush); color: var(--blush); background: rgba(212, 145, 122, 0.08); }

  /* How to use */
  .how-to {
    background: var(--warm);
    border-radius: 16px;
    padding: 36px 40px;
    margin-bottom: 70px;
    border: 1px solid var(--sand);
  }

  .how-to h2 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.5rem;
    font-weight: 400;
    color: var(--bark);
    margin-bottom: 16px;
  }

  .how-to-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
    margin-top: 20px;
  }

  .how-to-item {
    display: flex;
    gap: 14px;
    align-items: flex-start;
  }

  .how-to-icon {
    width: 34px;
    height: 34px;
    border-radius: 50%;
    background: var(--cream);
    border: 1px solid var(--sand);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 14px;
    flex-shrink: 0;
  }

  .how-to-item p {
    font-size: 13.5px;
    color: var(--muted);
    padding-top: 5px;
  }

  .how-to-item strong {
    color: var(--bark);
    font-weight: 500;
    display: block;
    font-size: 13px;
  }

  /* Week Section */
  .week {
    margin-bottom: 70px;
    animation: fadeUp 0.5s ease both;
  }

  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
  }

  .week-header {
    display: flex;
    align-items: flex-end;
    gap: 20px;
    margin-bottom: 8px;
  }

  .week-number {
    font-size: 11px;
    letter-spacing: 0.2em;
    text-transform: uppercase;
    color: var(--muted);
    padding-bottom: 2px;
  }

  .week-title {
    font-family: 'Cormorant Garamond', serif;
    font-size: 2rem;
    font-weight: 400;
    color: var(--bark);
    line-height: 1;
  }

  .week-theme {
    font-family: 'Cormorant Garamond', serif;
    font-style: italic;
    font-size: 14px;
    color: var(--muted);
    margin-bottom: 28px;
    padding-left: 2px;
  }

  .week-divider {
    height: 1px;
    background: linear-gradient(to right, var(--clay), transparent);
    margin-bottom: 28px;
    opacity: 0.4;
  }

  /* Day Card */
  .days-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 16px;
  }

  .day-card {
    background: white;
    border-radius: 14px;
    padding: 24px;
    border: 1px solid var(--sand);
    transition: transform 0.2s, box-shadow 0.2s;
    position: relative;
    overflow: hidden;
  }

  .day-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 3px;
  }

  .day-card.identity::before { background: linear-gradient(to right, var(--clay), var(--blush)); }
  .day-card.relationships::before { background: linear-gradient(to right, var(--blush), #e8a899); }
  .day-card.growth::before { background: linear-gradient(to right, var(--sage), #a8c5ac); }
  .day-card.integration::before { background: linear-gradient(to right, var(--earth), var(--clay)); }

  .day-card:hover {
    transform: translateY(-2px);
    box-shadow: 0 8px 24px rgba(74, 55, 40, 0.08);
  }

  .day-num {
    font-size: 11px;
    letter-spacing: 0.15em;
    text-transform: uppercase;
    color: var(--clay);
    margin-bottom: 10px;
    font-weight: 500;
  }

  .day-card.relationships .day-num { color: var(--blush); }
  .day-card.growth .day-num { color: var(--sage); }
  .day-card.integration .day-num { color: var(--earth); }

  .prompt-label {
    font-size: 10px;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--muted);
    margin-bottom: 5px;
    margin-top: 14px;
  }

  .prompt-label:first-of-type { margin-top: 0; }

  .prompt-text {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.05rem;
    line-height: 1.5;
    color: var(--ink);
  }

  .gratitude-prompt {
    font-size: 12.5px;
    color: var(--muted);
    font-style: italic;
    line-height: 1.5;
  }

  /* Weekly reflection */
  .weekly-reflection {
    margin-top: 24px;
    padding: 20px 24px;
    background: var(--warm);
    border-radius: 12px;
    border: 1px dashed var(--sand);
  }

  .weekly-reflection h4 {
    font-size: 11px;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    color: var(--clay);
    margin-bottom: 8px;
  }

  .weekly-reflection p {
    font-family: 'Cormorant Garamond', serif;
    font-size: 1.05rem;
    color: var(--bark);
    font-style: italic;
  }

  /* Closing */
  footer {
    text-align: center;
    padding-top: 60px;
    border-top: 1px solid var(--sand);
    margin-top: 20px;
  }

  footer h2 {
    font-family: 'Cormorant Garamond', serif;
    font-size: 2rem;
    font-weight: 300;
    color: var(--bark);
    margin-bottom: 16px;
  }

  footer p {
    font-size: 14px;
    color: var(--muted);
    max-width: 480px;
    margin: 0 auto;
    line-height: 1.8;
  }

  .closing-mark {
    font-size: 28px;
    color: var(--clay);
    margin-top: 32px;
    opacity: 0.5;
  }

  @media (max-width: 600px) {
    .page { padding: 40px 20px; }
    .days-grid { grid-template-columns: 1fr; }
    .how-to-grid { grid-template-columns: 1fr; }
    h1 { font-size: 2.4rem; }
  }
</style>
</head>
<body>
<div class="page">

  <header>
    <p class="subtitle">A Personal Journey · 30 Days</p>
    <h1>Know Yourself.<br><em>Grow</em> Yourself.<br>Connect Deeply.</h1>
    <p class="intro-text">A tailored journaling plan built around identity, personal growth, and the relationships that shape you — one prompt at a time.</p>
    <div class="tags">
      <span class="tag tag-identity">Identity</span>
      <span class="tag tag-growth">Personal Growth</span>
      <span class="tag tag-relationships">Relationships</span>
    </div>
  </header>

  <!-- How to use -->
  <div class="how-to">
    <h2>How to use this plan</h2>
    <p style="font-size:13.5px; color:var(--muted)">Each day has two parts: a <strong style="color:var(--clay)">Reflection Prompt</strong> to go deeper, and a <strong style="color:var(--sage)">Gratitude Prompt</strong> to anchor in what's good. You only need 10–15 minutes. There's no right or wrong — just write.</p>
    <div class="how-to-grid">
      <div class="how-to-item">
        <div class="how-to-icon">☀️</div>
        <p><strong>Same time, every day</strong>Morning or evening — pick one and stick to it.</p>
      </div>
      <div class="how-to-item">
        <div class="how-to-icon">✍️</div>
        <p><strong>Write without editing</strong>Don't judge what comes out. Let it flow freely.</p>
      </div>
      <div class="how-to-item">
        <div class="how-to-icon">🔒</div>
        <p><strong>This is just for you</strong>Write as if no one will ever read it. That's where honesty lives.</p>
      </div>
      <div class="how-to-item">
        <div class="how-to-icon">🔄</div>
        <p><strong>Missed a day? No guilt.</strong>Just pick up where you left off. Progress beats perfection.</p>
      </div>
    </div>
  </div>

  <!-- WEEK 1 -->
  <div class="week">
    <div class="week-header">
      <span class="week-number">Week One</span>
      <h2 class="week-title">Who Am I?</h2>
    </div>
    <p class="week-theme">Laying the foundation — exploring your values, stories, and the self you carry with you</p>
    <div class="week-divider"></div>
    <div class="days-grid">

      <div class="day-card identity">
        <div class="day-num">Day 1</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">If you had to describe yourself to a stranger using only 5 words, what would they be? Do you actually like those words?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">Name one thing about your personality you're genuinely glad you have.</p>
      </div>

      <div class="day-card identity">
        <div class="day-num">Day 2</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">What's a belief you've held your whole life that you've never really questioned? Where did it come from?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">What experience from your past are you grateful for, even if it was hard?</p>
      </div>

      <div class="day-card identity">
        <div class="day-num">Day 3</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">When do you feel most like yourself? What's happening in those moments — where are you, and who are you with?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">What is one small daily pleasure you never want to take for granted?</p>
      </div>

      <div class="day-card identity">
        <div class="day-num">Day 4</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">What are you most afraid people will find out about you? Why does that feel threatening?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">Who in your life accepts you as you are, flaws included? Write their name and why it matters.</p>
      </div>

      <div class="day-card identity">
        <div class="day-num">Day 5</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">What version of yourself are you performing for others that doesn't fully match who you are inside?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">What one thing did you do this week that you're quietly proud of?</p>
      </div>

      <div class="day-card identity">
        <div class="day-num">Day 6</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">If your 10-year-old self could see you today, what would surprise them most? What would disappoint them?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">What part of your childhood are you grateful still lives in you?</p>
      </div>

      <div class="day-card identity">
        <div class="day-num">Day 7</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">What do you want, independent of what anyone else wants for you? Write it without qualifying or apologizing for it.</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">What freedom in your life do you sometimes forget to appreciate?</p>
      </div>

    </div>
    <div class="weekly-reflection">
      <h4>End of Week 1 · Synthesis</h4>
      <p>"Reading back over this week — what's one word that describes the self you've been meeting on these pages?"</p>
    </div>
  </div>

  <!-- WEEK 2 -->
  <div class="week">
    <div class="week-header">
      <span class="week-number">Week Two</span>
      <h2 class="week-title">The People in My Life</h2>
    </div>
    <p class="week-theme">Examining your relationships — what they give you, what they cost you, and what they reveal about you</p>
    <div class="week-divider"></div>
    <div class="days-grid">

      <div class="day-card relationships">
        <div class="day-num">Day 8</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">Who in your life makes you feel the most seen and understood? What do they do that creates that feeling?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">Write three specific things a person in your life has done that you never properly thanked them for.</p>
      </div>

      <div class="day-card relationships">
        <div class="day-num">Day 9</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">Is there a relationship in your life that drains you? Without judgment — why do you think you stay in it?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">What has a difficult relationship taught you about yourself?</p>
      </div>

      <div class="day-card relationships">
        <div class="day-num">Day 10</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">How do you typically behave when you're in conflict with someone? What does that pattern say about what you need?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">Think of a conflict that eventually brought you closer to someone. What are you grateful for in that outcome?</p>
      </div>

      <div class="day-card relationships">
        <div class="day-num">Day 11</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">Is there someone you've been meaning to reach out to but haven't? What's the real reason you're hesitating?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">Who in your life is easy to overlook but would leave a real gap if they weren't there?</p>
      </div>

      <div class="day-card relationships">
        <div class="day-num">Day 12</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">How do you show love? How do you most need to receive it? Are the people around you aware of this?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">Recall one moment of genuine human connection you've had recently. What made it meaningful?</p>
      </div>

      <div class="day-card relationships">
        <div class="day-num">Day 13</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">What patterns from your family do you see repeating in your other relationships? Which ones do you want to break?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">What did someone in your family teach you — even indirectly — that you carry with pride?</p>
      </div>

      <div class="day-card relationships">
        <div class="day-num">Day 14</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">What kind of friend/partner/person do you want to be? How close are you to actually being that person?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">What relationship in your life are you most grateful exists, right now in this chapter?</p>
      </div>

    </div>
    <div class="weekly-reflection">
      <h4>End of Week 2 · Synthesis</h4>
      <p>"What's one small thing you could do this week to show up better in a relationship that matters to you?"</p>
    </div>
  </div>

  <!-- WEEK 3 -->
  <div class="week">
    <div class="week-header">
      <span class="week-number">Week Three</span>
      <h2 class="week-title">Growing Edges</h2>
    </div>
    <p class="week-theme">Leaning into your patterns, your resistance, and the places where real growth is waiting</p>
    <div class="week-divider"></div>
    <div class="days-grid">

      <div class="day-card growth">
        <div class="day-num">Day 15</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">What's something you keep saying you'll do "someday"? What would happen if someday were today?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">What resources — inner or outer — do you have right now to pursue what you want?</p>
      </div>

      <div class="day-card growth">
        <div class="day-num">Day 16</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">What does failure mean to you, and where did that definition come from? Is it serving you?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">Name a "failure" that, in hindsight, led somewhere better than your original plan.</p>
      </div>

      <div class="day-card growth">
        <div class="day-num">Day 17</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">Where do you tend to play it safe? What are you protecting yourself from by staying small in that area?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">What's a risk you took that you're glad you took, even if it was scary?</p>
      </div>

      <div class="day-card growth">
        <div class="day-num">Day 18</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">What emotion do you have the hardest time sitting with? What do you usually do to escape it?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">What's one thing your body does for you every day that you rarely acknowledge?</p>
      </div>

      <div class="day-card growth">
        <div class="day-num">Day 19</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">What habit or behavior do you know isn't serving you, but you keep returning to? What need is it meeting?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">What's a small win from this week — something you might normally dismiss as insignificant?</p>
      </div>

      <div class="day-card growth">
        <div class="day-num">Day 20</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">What story do you tell yourself about why your life is the way it is? How much of it is actually true?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">What has changed for the better in your life over the past year, however small?</p>
      </div>

      <div class="day-card growth">
        <div class="day-num">Day 21</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">If your wisest, most compassionate future self could give you one piece of advice right now, what would it be?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">What are three qualities you have that make you capable of growth?</p>
      </div>

    </div>
    <div class="weekly-reflection">
      <h4>End of Week 3 · Synthesis</h4>
      <p>"What's one belief or habit you're ready to let go of — and what would you like to replace it with?"</p>
    </div>
  </div>

  <!-- WEEK 4 -->
  <div class="week">
    <div class="week-header">
      <span class="week-number">Week Four</span>
      <h2 class="week-title">Becoming</h2>
    </div>
    <p class="week-theme">Integrating everything — articulating your values, your direction, and the person you're choosing to become</p>
    <div class="week-divider"></div>
    <div class="days-grid">

      <div class="day-card integration">
        <div class="day-num">Day 22</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">What does a life well-lived look like to you — not in terms of achievements, but in terms of how it feels day to day?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">How many elements of that life do you already have access to right now?</p>
      </div>

      <div class="day-card integration">
        <div class="day-num">Day 23</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">What are your top 3 personal values? Do the choices you make daily actually reflect them?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">When did you recently act in alignment with one of your values? How did it feel?</p>
      </div>

      <div class="day-card integration">
        <div class="day-num">Day 24</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">What do you want the people closest to you to remember about you? Are you living in a way that creates those memories?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">Who has shown you what it looks like to live with integrity or kindness?</p>
      </div>

      <div class="day-card integration">
        <div class="day-num">Day 25</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">Where are you currently investing energy that isn't aligned with where you want to go? What would it look like to redirect it?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">What opportunity is currently open to you that you might be underestimating?</p>
      </div>

      <div class="day-card integration">
        <div class="day-num">Day 26</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">Write a letter to yourself from 5 years in the future. What has changed? What stayed the same? What are you glad you started?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">What's a quality about yourself that you've come to appreciate more as you've gotten older?</p>
      </div>

      <div class="day-card integration">
        <div class="day-num">Day 27</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">What does self-compassion look like for you specifically? In what areas do you find it hardest to extend to yourself?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">Write one kind, true thing about yourself that you rarely let yourself fully believe.</p>
      </div>

      <div class="day-card integration">
        <div class="day-num">Day 28</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">What one relationship do you want to deepen or repair in the next season of your life? What's your first step?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">What connection have you built or strengthened this month that you're grateful for?</p>
      </div>

      <div class="day-card integration">
        <div class="day-num">Day 29</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">Who are you becoming? Not who you should be — who are you actually, slowly, becoming?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">What about your life right now — this exact chapter — will you one day look back on with warmth?</p>
      </div>

      <div class="day-card integration">
        <div class="day-num">Day 30</div>
        <div class="prompt-label">Reflection</div>
        <p class="prompt-text">What has this month of journaling revealed that you didn't know, or didn't want to admit, before you started?</p>
        <div class="prompt-label">Gratitude</div>
        <p class="gratitude-prompt">Write a note of gratitude to yourself for showing up for 30 days. Mean every word of it.</p>
      </div>

    </div>
    <div class="weekly-reflection">
      <h4>End of Week 4 · Synthesis</h4>
      <p>"If you had to name one thing that has genuinely shifted in how you see yourself after these 30 days — what is it?"</p>
    </div>
  </div>

  <footer>
    <h2>The journal doesn't end here.</h2>
    <p>30 days is just the beginning of a conversation with yourself. The questions get deeper, the answers get more honest, and you get more comfortable not always having them. Keep going.</p>
    <div class="closing-mark">✦</div>
  </footer>

</div>
</body>
</html>


