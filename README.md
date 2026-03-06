# D.React-Step-Project- +vite + TailwindCss 
How to creat React Step Project 

1 Install node on terminal vwindow in your computer type  , brew install node 
2(check the version node -v , nmp -v )

Explanation

Node.js → the runtime that lets you run JavaScript on your Mac (outside the browser)

npm (Node Package Manager) → the tool that comes with Node.js to install, manage, and run packages/libraries for your projects

So if you install Node.js, npm is automatically installed too. You don’t need to install it separately.

----------------
opetion2 Option 2: Install from Node.js website

Go to https://nodejs.org

Download the LTS version (recommended) for macOS

Open the .pkg file and follow the installer steps

Verify installation in Terminal. 

------------------------------------------------------------------
Step 3: Create a project folder and open your terminal window 
----------------------------------------------------------------------
Step 3:  Create a  React project with the latest version of Vite, navigate your project folder  type in the terminal window 
npm create vite@latest my-react-app     ok or enter.

The command will ask a few questions:

Project name → press Enter (or type a new name)

Framework → choose React

Variant → choose JavaScript (not TypeScript if you want plain JS)
So Vite will now generate your React project. done 

------------------------------------------------------------------
4 , type 
cd my-react-app 

5. Install the npm command 
npm install

6 , type  npm run dev 

7,VITE v5.x.x  ready in 300ms
Local:   http://localhost:5173/,   so copy the URL and paste it in your browser to see your page 
If you want to stop running, just type combine control + c  and enter or ok 

----------------------------
add now TailwindCss 
got to this tailwindcss.com and click on Docs 
https://tailwindcss.com/docs/installation/using-vite

follow the step  , type in your terminal windows :
=> npm install tailwindcss @tailwindcss/vite   
it will create this fike (vite.config.ts)
Configure the Vite plugin
Add the @tailwindcss/vite plugin to your Vite configuration.

import { defineConfig } from 'vite'
import tailwindcss from '@tailwindcss/vite'
import react from '@vitejs/plugin-react'
export default defineConfig({
  plugins: [
    react(),
    tailwindcss(),
  ],
})



after this go to your Css file and clear up all content and 
Add an @import to your CSS file that imports Tailwind CSS.
=>  @import "tailwindcss";


after write this code in app.jsx file 
 <div>
      <h1 className="text-3xl font-bold underline">
        Hello world!
      </h1>
      <p>Vite + React</p>
      <div className="card">
        <button onClick={() => setCount((c) => c + 1)}>
          count is {count}
        </button>
      </div>
    </div>

--------------




