* Recommended File Structure *

src/
      ├─ app/
          ├─ layout.js              → Root layout (fonts, navbar, sidebar)
          ├─ globals.css
   
          ├─ page.jsx               → Public landing / dashboard
   
          ├─ dashboard/
               └─ page.jsx           → CMS dashboard main page
   
          ├─ posts/
               └─ page.jsx           → List of posts
   
         ├─ posts/[id]/
              └─ page.jsx           → Single post edit/view
   
         ├─ settings/
              └─ page.jsx           → CMS settings
   
         └─ api/                   → Later (optional backend APIs)

    ├─ components/
         ├─ layout/
             ├─ Navbar.jsx         → Top bar (logo, profile)
             ├─ Sidebar.jsx        → Side navigation
             └─ Footer.jsx
   
         ├─ ui/
             ├─ Button.jsx
             ├─ Input.jsx
             └─ Card.jsx
   
        └─ common/
             └─ Logo.jsx
   
        ├─ lib/
            └─ constants.js           → Menu items, roles

└─ public/
     └─ logo.png               → Logo





* app/layout.js (Global Shell) *

    This file should contain:
    
      <Navbar />
      
      <Sidebar />
      
      <main>{children}</main>
    
    Meaning:
    
      Navbar & Sidebar never reload
      
      Only page content changes

  * Navbar (Top) *

         Logo
         
         User profile
         
         Logout
         
         Notifications
   
         // components/layout/Navbar.jsx

   * Sidebar (Left) *

         Dashboard
   
         Posts
         
         Pages
         
         Media
         
         Settings
   
         // components/layout/Sidebar.jsx




