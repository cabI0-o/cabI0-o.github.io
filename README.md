# Karylle G. Cabrido.

### education
fnujewf
### work experience
fvefvv
import { useState } from "react";

const Portfolio = () => {
  const [activeSection, setActiveSection] = useState("home");

  const scrollToSection = (sectionId: string) => {
    const element = document.getElementById(sectionId);
    if (element) {
      element.scrollIntoView({ behavior: "smooth" });
      setActiveSection(sectionId);
    }
  };

  return (
    <div className="min-h-screen bg-background text-foreground font-sans">
      {/* Header Navigation */}
      <header className="fixed top-0 w-full bg-background/90 backdrop-blur-sm z-50 border-b border-border">
        <nav className="container mx-auto px-6 py-4">
          <div className="flex justify-between items-center">
            <div className="text-xl font-bold text-primary">John Doe</div>
            <div className="hidden md:flex space-x-8">
              <button
                onClick={() => scrollToSection("home")}
                className={`hover:text-primary transition-colors ${
                  activeSection === "home" ? "text-primary" : "text-foreground"
                }`}
              >
                Home
              </button>
                <button
                onClick={() => scrollToSection("about")}
                className={`hover:text-primary transition-colors ${
                  activeSection === "about" ? "text-primary" : "text-foreground"
                }`}
              >
                About
              </button>
              <button
                onClick={() => scrollToSection("skills")}
                className={`hover:text-primary transition-colors ${
                  activeSection === "skills" ? "text-primary" : "text-foreground"
                }`}
              >
                Skills
              </button>
              <button
                onClick={() => scrollToSection("projects")}
                className={`hover:text-primary transition-colors ${
                  activeSection === "projects" ? "text-primary" : "text-foreground"
                }`}
              >
                Projects
              </button>
              <button
                onClick={() => scrollToSection("contact")}
                className={`hover:text-primary transition-colors ${
                  activeSection === "contact" ? "text-primary" : "text-foreground"
                }`}
              >
                Contact
              </button>
            </div>
            <button className="md:hidden text-foreground">
              <svg className="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M4 6h16M4 12h16M4 18h16" />
              </svg>
            </button>
          </div>
        </nav>
      </header>

      {/* Hero Section */}
      <section id="home" className="min-h-screen flex items-center justify-center pt-20 pb-16">
        <div className="container mx-auto px-6 text-center">
          <div className="max-w-2xl mx-auto">
            <div className="mb-8">
              <img 
                src="https://placeholder-image-service.onrender.com/image/200x200?prompt=Professional headshot of a software developer with friendly expression&id=portfolio-avatar" 
                alt="Professional headshot of John Doe, a software developer" 
                className="w-32 h-32 rounded-full mx-auto mb-6 object-cover border-4 border-primary"
              />
            </div>
            <h1 className="text-4xl md:text-6xl font-bold mb-6 text-foreground">
              Hi, I'm <span className="text-primary">John Doe</span>
            </h1>
            <p className="text-xl md:text-2xl text-muted-foreground mb-8">
              Full Stack Developer & UI/UX Enthusiast
            </p>
            <p className="text-lg text-muted-foreground mb-10">
              Creating beautiful, functional, and user-centered digital experiences
            </p>
            <div className="flex flex-col sm:flex-row gap-4 justify-center">
              <button 
                onClick={() => scrollToSection("projects")}
                className="px-8 py-3 bg-primary text-primary-foreground rounded-lg hover:bg-primary/90 transition-colors font-medium"
              >
                View My Work
              </button>
              <button 
                onClick={() => scrollToSection("contact")}
                className="px-8 py-3 border border-primary text-primary rounded-lg hover:bg-primary hover:text-primary-foreground transition-colors font-medium"
              >
                Contact Me
              </button>
            </div>
          </div>
        </div>
      </section>

      {/* About Section */}
      <section id="about" className="py-20 bg-muted/30">
        <div className="container mx-auto px-6">
          <div className="max-w-4xl mx-auto">
            <h2 className="text-3xl md:text-4xl font-bold text-center mb-12 text-foreground">About Me</h2>
            <div className="grid md:grid-cols-2 gap-12 items-center">
              <div>
                <img 
                  src="https://placeholder-image-service.onrender.com/image/400x500?prompt=Developer working at desk with computer and coffee&id=about-section" 
                  alt="John Doe working at his desk with computer and coffee, showing professional work environment" 
                  className="rounded-lg shadow-lg w-full h-auto"
                />
              </div>
              <div>
                <p className="text-lg text-muted-foreground mb-6">
                  I'm a passionate full-stack developer with over 5 years of experience creating 
                  digital solutions that make a difference. I specialize in React, TypeScript, 
                  and modern web development practices.
                </p>
                <p className="text-lg text-muted-foreground mb-6">
                  My approach combines technical expertise with a keen eye for design, ensuring 
                  that every project is not only functional but also provides an exceptional 
                  user experience.
                </p>
                <p className="text-lg text-muted-foreground">
                  When I'm not coding, you can find me exploring new technologies, contributing 
                  to open source projects, or enjoying outdoor activities.
                </p>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Skills Section */}
      <section id="skills" className="py-20">
        <div className="container mx-auto px-6">
          <h2 className="text-3xl md:text-4xl font-bold text-center mb-16 text-foreground">Skills & Technologies</h2>
          <div className="grid grid-cols-2 md:grid-cols-4 gap-6 max-w-4xl mx-auto">
            {/* Skill Item 1 */}
            <div className="text-center p-6 bg-card rounded-lg shadow-sm hover:shadow-md transition-shadow">
              <div className="w-16 h-16 mx-auto mb-4 bg-primary/10 rounded-full flex items-center justify-center">
                <svg className="w-8 h-8 text-primary" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4" />
                </svg>
              </div>
              <h3 className="font-semibold mb-2">React</h3>
              <p className="text-sm text-muted-foreground">Frontend Development</p>
            </div>

            {/* Skill Item 2 */}
            <div className="text-center p-6 bg-card rounded-lg shadow-sm hover:shadow-md transition-shadow">
              <div className="w-16 h-16 mx-auto mb-4 bg-primary/10 rounded-full flex items-center justify-center">
                <svg className="w-8 h-8 text-primary" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M13 10V3L4 14h7v7l9-11h-7z" />
                </svg>
              </div>
              <h3 className="font-semibold mb-2">TypeScript</h3>
              <p className="text-sm text-muted-foreground">Type Safety</p>
            </div>

            {/* Skill Item 3 */}
            <div className="text-center p-6 bg-card rounded-lg shadow-sm hover:shadow-md transition-shadow">
              <div className="w-16 h-16 mx-auto mb-4 bg-primary/10 rounded-full flex items-center justify-center">
                <svg className="w-8 h-8 text-primary" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M4 5a1 1 0 011-1h14a1 1 0 011 1v2a1 1 0 01-1 1H5a1 1 0 01-1-1V5zM4 13a1 1 0 011-1h6a1 1 0 011 1v6a1 1 0 01-1 1H5a1 1 0 01-1-1v-6zM16 13a1 1 0 011-1h2a1 1 0 011 1v6a1 1 0 01-1 1h-2a1 1 0 01-1-1v-6z" />
                </svg>
              </div>
              <h3 className="font-semibold mb-2">Node.js</h3>
              <p className="text-sm text-muted-foreground">Backend Development</p>
            </div>

            {/* Skill Item 4 */}
            <div className="text-center p-6 bg-card rounded-lg shadow-sm hover:shadow-md transition-shadow">
              <div className="w-16 h-16 mx-auto mb-4 bg-primary/10 rounded-full flex items-center justify-center">
                <svg className="w-8 h-8 text-primary" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M12 6V4m0 2a2 2 0 100 4m0-4a2 2 0 110 4m-6 8a2 2 0 100-4m0 4a2 2 0 100 4m0-4v2m0-6V4m6 6v10m6-2a2 2 0 100-4m0 4a2 2 0 100 4m0-4v2m0-6V4" />
                </svg>
              </div>
              <h3 className="font-semibold mb-2">Tailwind CSS</h3>
              <p className="text-sm text-muted-foreground">Styling</p>
            </div>
          </div>
        </div>
      </section>

      {/* Projects Section */}
      <section id="projects" className="py-20 bg-muted/30">
        <div className="container mx-auto px-6">
          <h2 className="text-3xl md:text-4xl font-bold text-center mb-16 text-foreground">Featured Projects</h2>
          <div className="grid md:grid-cols-2 lg:grid-cols-3 gap-8 max-w-6xl mx-auto">
            {/* Project 1 */}
            <div className="bg-card rounded-lg overflow-hidden shadow-sm hover:shadow-lg transition-shadow">
              <img 
                src="https://placeholder-image-service.onrender.com/image/400x250?prompt=E-commerce website dashboard with product listings and analytics&id=project-ecommerce" 
                alt="E-commerce dashboard interface showing product listings, analytics charts, and order management system" 
                className="w-full h-48 object-cover"
              />
              <div className="p-6">
                <h3 className="text-xl font-semibold mb-2">E-Commerce Platform</h3>
                <p className="text-muted-foreground mb-4">
                  A full-stack e-commerce solution with React, Node.js, and MongoDB.
                </p>
                <div className="flex flex-wrap gap-2 mb-4">
                  <span className="px-3 py-1 bg-primary/10 text-primary text-sm rounded-full">React</span>
                  <span className="px-3 py-1 bg-primary/10 text-primary text-sm rounded-full">Node.js</span>
                  <span className="px-3 py-1 bg-primary/10 text-primary text-sm rounded-full">MongoDB</span>
                </div>
                <div className="flex space-x-4">
                  <button className="text-primary hover:underline text-sm">Live Demo</button>
                  <button className="text-primary hover:underline text-sm">GitHub</button>
                </div>
              </div>
            </div>

            {/* Project 2 */}
            <div className="bg-card rounded-lg overflow-hidden shadow-sm hover:shadow-lg transition-shadow">
              <img 
                src="https://placeholder-image-service.onrender.com/image/400x250?prompt=Task management application with kanban board and calendar view&id=project-taskmanager" 
                alt="Task management application interface with kanban board, drag and drop functionality, and calendar integration" 
                className="w-full h-48 object-cover"
              />
              <div className="p-6">
                <h3 className="text-xl font-semibold mb-2">Task Management App</h3>
                <p className="text-muted-foreground mb-4">
                  Collaborative task management with real-time updates and drag-and-drop.
                </p>
                <div className="flex flex-wrap gap-2 mb-4">
                  <span className="px-3 py-1 bg-primary/10 text-primary text-sm rounded-full">React</span>
                  <span className="px-3 py-1 bg-primary/10 text-primary text-sm rounded-full">Firebase</span>
                  <span className="px-3 py-1 bg-primary/10 text-primary text-sm rounded-full">Tailwind</span>
                </div>
                <div className="flex space-x-4">
                  <button className="text-primary hover:underline text-sm">Live Demo</button>
                  <button className="text-primary hover:underline text-sm">GitHub</button>
                </div>
              </div>
            </div>

            {/* Project 3 */}
            <div className="bg-card rounded-lg overflow-hidden shadow-sm hover:shadow-lg transition-shadow">
              <img 
                src="https://placeholder-image-service.onrender.com/image/400x250?prompt=Weather application dashboard with forecast charts and location search&id=project-weather" 
                alt="Weather application interface showing current conditions, 7-day forecast, and interactive weather maps" 
                className="w-full h-48 object-cover"
              />
              <div className="p-6">
                <h3 className="text-xl font-semibold mb-2">Weather Dashboard</h3>
                <p className="text-muted-foreground mb-4">
                  Real-time weather information with beautiful data visualizations.
                </p>
                <div className="flex flex-wrap gap-2 mb-4">
                  <span className="px-3 py-1 bg-primary/10 text-primary text-sm rounded-full">Vue.js</span>
                  <span className="px-3 py-1 bg-primary/10 text-primary text-sm rounded-full">Chart.js</span>
                  <span className="px-3 py-1 bg-primary/10 text-primary text-sm rounded-full">API</span>
                </div>
                <div className="flex space-x-4">
                  <button className="text-primary hover:underline text-sm">Live Demo</button>
                  <button className="text-primary hover:underline text-sm">GitHub</button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Contact Section */}
      <section id="contact" className="py-20">
        <div className="container mx-auto px-6">
          <div className="max-w-2xl mx-auto text-center">
            <h2 className="text-3xl md:text-4xl font-bold mb-8 text-foreground">Get In Touch</h2>
            <p className="text-lg text-muted-foreground mb-12">
              I'm always interested in new opportunities and collaborations. 
              Let's talk about how we can work together!
            </p>
            <form className="space-y-6 text-left">
              <div>
                <label htmlFor="name" className="block text-sm font-medium mb-2">Name</label>
                <input 
                  type="text" 
                  id="name" 
                  className="w-full px-4 py-3 border border-border rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent"
                  placeholder="Your name"
                />
              </div>
              <div>
                <label htmlFor="email" className="block text-sm font-medium mb-2">Email</label>
                <input 
                  type="email" 
                  id="email" 
                  className="w-full px-4 py-3 border border-border rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent"
                  placeholder="your.email@example.com"
                />
              </div>
              <div>
                <label htmlFor="message" className="block text-sm font-medium mb-2">Message</label>
                <textarea 
                  id="message" 
                  rows={5}
                  className="w-full px-4 py-3 border border-border rounded-lg focus:ring-2 focus:ring-primary focus:border-transparent"
                  placeholder="Your message here..."
                ></textarea>
              </div>
              <button 
                type="submit"
                className="w-full bg-primary text-primary-foreground py-3 px-6 rounded-lg hover:bg-primary/90 transition-colors font-medium"
              >
                Send Message
              </button>
            </form>
          </div>
        </div>
      </section>

      {/* Footer */}
      <footer className="bg-muted py-12">
        <div className="container mx-auto px-6 text-center">
          <div className="flex justify-center space-x-6 mb-6">
            <a href="#" className="text-muted-foreground hover:text-primary transition-colors">
              <svg className="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
              </svg>
            </a>
            <a href="#" className="text-muted-foreground hover:text-primary transition-colors">
              <svg className="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                <path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/>
              </svg>
            </a>
            <a href="#" className="text-muted-foreground hover:text-primary transition-colors">
              <svg className="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                <path d="M23.953 4.57a10 10 0 01-2.825.775 4.958 4.958 0 002.163-2.723c-.951.555-2.005.959-3.127 1.184a4.92 4.92 0 00-8.384 4.482C7.69 8.095 4.067 6.13 1.64 3.162a4.822 4.822 0 00-.666 2.475c0 1.71.87 3.213 2.188 4.096a4.904 4.904 0 01-2.228-.616v.06a4.923 4.923 0 003.946 4.827 4.996 4.996 0 01-2.212.085 4.936 4.936 0 004.604 3.417 9.867 9.867 0 01-6.102 2.105c-.39 0-.779-.023-1.17-.067a13.995 13.995 0 007.557 2.209c9.053 0 13.998-7.496 13.998-13.985 0-.21 0-.42-.015-.63A9.935 9.935 0 0024 4.59z"/>
              </svg>
            </a>
          </div>
          <p className="text-muted-foreground">
            © 2024 John Doe. All rights reserved.
          </p>
        </div>
      </footer>
    </div>
  );
};

export default Portfolio;
