```aura width=860 height=320
<div style={{
  width: '100%', height: '100%', background: '#06060a',
  display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center',
  fontFamily: 'Inter, sans-serif', position: 'relative', overflow: 'hidden',
  borderRadius: 20, border: '1px solid rgba(0,229,255,0.08)'
}}>

  <style>{`
    @keyframes hero-orb-a { 0%, 100% { transform: translate(0,0); opacity: 0.55; } 50% { transform: translate(40px,-30px); opacity: 0.85; } }
    @keyframes hero-orb-b { 0%, 100% { transform: translate(0,0); opacity: 0.45; } 50% { transform: translate(-35px,25px); opacity: 0.75; } }
    @keyframes hero-orb-c { 0%, 100% { transform: translate(0,0); opacity: 0.35; } 50% { transform: translate(25px,-40px); opacity: 0.65; } }
    @keyframes hero-orb-d { 0%, 100% { transform: translate(0,0); opacity: 0.40; } 50% { transform: translate(-20px,-15px); opacity: 0.70; } }
    @keyframes hero-ring { 0%, 100% { opacity: 0.04; } 50% { opacity: 0.14; } }
    @keyframes hero-ring-b { 0%, 100% { opacity: 0.03; } 50% { opacity: 0.10; } }
    @keyframes hero-dot-spin { 0% { transform: rotate(0deg); } 100% { transform: rotate(360deg); } }
    @keyframes hero-line-scan { 0% { transform: translateY(-320px); } 100% { transform: translateY(320px); } }
    @keyframes hero-cursor { 0%, 100% { opacity: 1; } 49% { opacity: 1; } 50% { opacity: 0; } 99% { opacity: 0; } }
    #ho1 { animation: hero-orb-a 9s ease-in-out infinite; }
    #ho2 { animation: hero-orb-b 12s ease-in-out infinite 0.6s; }
    #ho3 { animation: hero-orb-c 8s ease-in-out infinite 1.5s; }
    #ho4 { animation: hero-orb-d 11s ease-in-out infinite 0.3s; }
    #ho5 { animation: hero-orb-a 10s ease-in-out infinite 2s; }
    #ho6 { animation: hero-orb-b 14s ease-in-out infinite 1s; }
    #hr1 { animation: hero-ring 9s ease-in-out infinite; }
    #hr2 { animation: hero-ring 9s ease-in-out infinite 1.5s; }
    #hr3 { animation: hero-ring-b 9s ease-in-out infinite 3s; }
    #hr4 { animation: hero-ring-b 10s ease-in-out infinite 4.5s; }
    #hdot { animation: hero-dot-spin 24s linear infinite; }
    #hscan { animation: hero-line-scan 6s linear infinite; }
    #hcur { animation: hero-cursor 1.1s step-end infinite; }
  `}</style>

  <svg width="860" height="320" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="hg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(0,229,255,0.50)" />
        <stop offset="60%" stopColor="rgba(0,229,255,0.12)" />
        <stop offset="100%" stopColor="rgba(0,229,255,0)" />
      </radialGradient>
      <radialGradient id="hg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(139,92,246,0.55)" />
        <stop offset="55%" stopColor="rgba(139,92,246,0.15)" />
        <stop offset="100%" stopColor="rgba(139,92,246,0)" />
      </radialGradient>
      <radialGradient id="hg3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(51,102,255,0.45)" />
        <stop offset="60%" stopColor="rgba(51,102,255,0.10)" />
        <stop offset="100%" stopColor="rgba(51,102,255,0)" />
      </radialGradient>
      <radialGradient id="hg4" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(236,72,153,0.30)" />
        <stop offset="70%" stopColor="rgba(236,72,153,0)" />
      </radialGradient>
      <radialGradient id="hg5" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(0,180,255,0.35)" />
        <stop offset="100%" stopColor="rgba(0,180,255,0)" />
      </radialGradient>
      <radialGradient id="hg6" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(168,85,247,0.40)" />
        <stop offset="100%" stopColor="rgba(168,85,247,0)" />
      </radialGradient>
      <linearGradient id="hscan-g" x1="0" y1="0" x2="0" y2="1">
        <stop offset="0%" stopColor="rgba(0,229,255,0)" />
        <stop offset="45%" stopColor="rgba(0,229,255,0.04)" />
        <stop offset="50%" stopColor="rgba(0,229,255,0.12)" />
        <stop offset="55%" stopColor="rgba(0,229,255,0.04)" />
        <stop offset="100%" stopColor="rgba(0,229,255,0)" />
      </linearGradient>
    </defs>

    <ellipse id="ho1" cx="120" cy="280" rx="280" ry="200" fill="url(#hg1)" />
    <ellipse id="ho2" cx="740" cy="60"  rx="250" ry="190" fill="url(#hg2)" />
    <ellipse id="ho3" cx="430" cy="310" rx="200" ry="160" fill="url(#hg3)" />
    <ellipse id="ho4" cx="680" cy="290" rx="180" ry="140" fill="url(#hg4)" />
    <ellipse id="ho5" cx="250" cy="40"  rx="220" ry="160" fill="url(#hg5)" />
    <ellipse id="ho6" cx="500" cy="60"  rx="160" ry="130" fill="url(#hg6)" />

    <circle id="hr1" cx="430" cy="160" r="55"  fill="none" stroke="rgba(0,229,255,0.7)" strokeWidth="0.5" />
    <circle id="hr2" cx="430" cy="160" r="100" fill="none" stroke="rgba(139,92,246,0.6)" strokeWidth="0.5" />
    <circle id="hr3" cx="430" cy="160" r="155" fill="none" stroke="rgba(51,102,255,0.5)" strokeWidth="0.4" />
    <circle id="hr4" cx="430" cy="160" r="220" fill="none" stroke="rgba(0,229,255,0.3)" strokeWidth="0.3" />

    <g id="hdot">
      <circle cx="430" cy="105" r="2" fill="rgba(0,229,255,0.6)" />
    </g>

    <rect id="hscan" x="0" y="0" width="860" height="320" fill="url(#hscan-g)" />
  </svg>

  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', zIndex: 10 }}>
    <span style={{
      fontSize: 11, letterSpacing: 6, textTransform: 'uppercase',
      color: 'rgba(0,229,255,0.50)', fontWeight: 300, marginBottom: 14
    }}>full stack engineer</span>

    <span style={{
      fontSize: 52, fontWeight: 800, letterSpacing: -2, lineHeight: 1,
      color: '#ffffff',
      textShadow: '0 0 60px rgba(0,229,255,0.25), 0 0 120px rgba(139,92,246,0.15)'
    }}>Aditya Vikram Singh</span>

    <div style={{ display: 'flex', alignItems: 'center', marginTop: 16, gap: 6 }}>
      <span style={{
        fontSize: 15, color: 'rgba(180,190,255,0.70)', fontWeight: 400,
        letterSpacing: 0.5, fontFamily: 'monospace'
      }}>> Scalable frontends · AI-assisted systems · Enterprise platforms</span>
      <span id="hcur" style={{ fontSize: 15, color: 'rgba(0,229,255,0.7)', fontFamily: 'monospace' }}>_</span>
    </div>

    <div style={{ display: 'flex', gap: 8, marginTop: 24, flexWrap: 'wrap', justifyContent: 'center' }}>
      {['Scalable Frontend Architecture', 'Performance Engineering', 'AI-Assisted Systems', 'Observability & Dashboards'].map(function(tag, i) {
        return (
          <span key={i} style={{
            padding: '5px 14px', borderRadius: 100,
            background: 'rgba(0,229,255,0.04)',
            border: '1px solid rgba(0,229,255,0.12)',
            color: 'rgba(0,229,255,0.65)', fontSize: 11, fontWeight: 500, letterSpacing: 0.8
          }}>{tag}</span>
        );
      })}
    </div>
  </div>
</div>
```
