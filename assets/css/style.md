/* ========================
   🖋️ Klassisch & Minimal: Monochromes Blau-Größe-Spektrum
   ======================== */

body {
  font-family: 'Inter', 'Segoe UI', 'Helvetica Neue', Arial, sans-serif;
  line-height: 1.7;
  color: #1a1a1a;
  background-color: #f8f9fa;
  margin: 0;
  padding: 0;
}

h1, h2, h3, h4 {
  font-weight: 600;
  letter-spacing: -0.02em;
  margin-top: 0;
  margin-bottom: 0.5em;
}

h1 {
  font-size: 2.4rem;
  color: #0f2a45;
  margin-bottom: 10px;
}

h2 {
  font-size: 1.8rem;
  color: #0f2a45;
  border-bottom: 1px solid #d0d0d0;
  padding-bottom: 8px;
  margin-top: 40px;
}

h3 {
  font-size: 1.4rem;
  color: #1a3a5f;
  margin-top: 25px;
}

.container {
  max-width: 1000px;
  margin: 0 auto;
  padding: 40px 20px;
}

/* ========================
   🔗 Navigation
   ======================== */
nav ul {
  list-style: none;
  padding: 0;
  margin: 20px 0;
  display: flex;
  justify-content: center;
  gap: 30px;
  flex-wrap: wrap;
}

nav a {
  color: #1a3a5f;
  text-decoration: none;
  font-size: 1.05rem;
  font-weight: 500;
  transition: color 0.3s ease, transform 0.2s ease;
  position: relative;
  padding-bottom: 4px;
}

nav a:hover {
  color: #0f2a45;
  transform: translateY(-1px);
}

nav a::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 0;
  height: 1px;
  background-color: #0f2a45;
  transition: width 0.3s ease;
}

nav a:hover::after {
  width: 100%;
}

/* ========================
   🎯 Startseite: Buttons
   ======================== */
section {
  margin-top: 50px;
  text-align: center;
}

section a {
  display: inline-block;
  padding: 14px 32px;
  background-color: #1a3a5f;
  color: white;
  text-decoration: none;
  border-radius: 6px;
  font-size: 1.1rem;
  font-weight: 600;
  letter-spacing: 0.02em;
  transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
  border: 1px solid transparent;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
}

section a:hover {
  background-color: #0f2a45;
  transform: translateY(-2px);
  box-shadow: 0 6px 16px rgba(0, 0, 0, 0.12);
  border-color: #0f2a45;
}

/* ========================
   🖼️ Logos
   ======================== */
.partner-logos {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 30px;
  margin-top: 40px;
  padding: 20px;
  background-color: #ffffff;
  border-radius: 12px;
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.05);
}

.partner-logos img {
  height: 80px;
  object-fit: contain;
  transition: transform 0.3s ease;
  border-radius: 6px;
  border: 1px solid #e0e0e0;
}

.partner-logos img:hover {
  transform: scale(1.05);
  box-shadow: 0 6px 16px rgba(0, 0, 0, 0.1);
}

/* ========================
   📚 Tabellen (Team)
   ======================== */
table {
  width: 100%;
  border-collapse: collapse;
  margin-top: 20px;
  background-color: #ffffff;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);
}

th, td {
  padding: 14px 16px;
  text-align: left;
  border-bottom: 1px solid #e0e0e0;
}

th {
  background-color: #f2f5f9;
  color: #0f2a45;
  font-weight: 600;
  font-size: 0.95rem;
}

tr:hover {
  background-color: #f8f9fa;
}

a {
  color: #1a3a5f;
  text-decoration: none;
  transition: color 0.3s ease;
}

a:hover {
  color: #0f2a45;
  text-decoration: underline;
}

/* ========================
   📄 Footer
   ======================== */
footer {
  text-align: center;
  margin-top: 60px;
  padding: 25px;
  background-color: #0f2a45;
  color: #e0e0e0;
  font-size: 0.9rem;
  border-top: 1px solid #1a3a5f;
}

footer a {
  color: #66aaff;
  text-decoration: none;
}

footer a:hover {
  text-decoration: underline;
}

/* ========================
   📱 Responsive
   ======================== */
@media (max-width: 768px) {
  h1 {
    font-size: 2rem;
  }

  h2 {
    font-size: 1.5rem;
  }

  nav ul {
    gap: 15px;
    flex-direction: column;
    align-items: center;
  }

  section a {
    padding: 12px 24px;
    font-size: 1rem;
  }

  .partner-logos {
    gap: 20px;
    padding: 15px;
  }

  .partner-logos img {
    height: 60px;
  }
}