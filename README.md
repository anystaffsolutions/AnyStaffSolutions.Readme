// Full immersive onboarding portal with AI chat, PPE, and uniform system // Includes dressing room view, Amazon affiliate link, and custom design submission // Ready for GitHub push + Netlify deployment

import React, { useState } from 'react'; import { motion } from 'framer-motion'; import ChatBox from './components/ChatBox'; import DressingRoom from './components/DressingRoom'; import BedroomBackground from './assets/bedroom.jpg'; import ClosetBackground from './assets/closet.jpg';

export default function AnyStaffPortal() { const [showChat, setShowChat] = useState(false); const [showDressingRoom, setShowDressingRoom] = useState(false);

return ( <div className="relative w-screen h-screen bg-cover bg-center" style={{ backgroundImage: url(${BedroomBackground}) }} > {/* Laptop to open chat */} <motion.div initial={{ opacity: 0, y: -20 }} animate={{ opacity: 1, y: 0 }} transition={{ delay: 1.5, duration: 0.5 }} className="absolute top-4 right-4 w-64 h-40 bg-gray-800 rounded-md shadow-lg cursor-pointer" onClick={() => setShowChat(true)} > <div className="w-full h-full flex items-center justify-center text-white text-sm"> 💻 Open Co-Pilot </div> </motion.div>

{/* Chat box */}
  {showChat && (
    <motion.div
      initial={{ opacity: 0, scale: 0.9 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={{ duration: 0.3 }}
      className="absolute top-4 right-4 w-96 h-96 bg-white border-2 border-gray-300 rounded-xl overflow-hidden z-50"
    >
      <ChatBox />
    </motion.div>
  )}

  {/* Button to open dressing room */}
  <motion.div
    initial={{ opacity: 0, y: 20 }}
    animate={{ opacity: 1, y: 0 }}
    transition={{ delay: 2, duration: 0.5 }}
    className="absolute bottom-6 left-6 bg-white px-4 py-2 rounded-md shadow cursor-pointer"
    onClick={() => setShowDressingRoom(true)}
  >
    🎽 Go to Dressing Room
  </motion.div>

  {/* Dressing room view */}
  {showDressingRoom && (
    <div
      className="absolute inset-0 w-screen h-screen bg-cover bg-center z-40"
      style={{ backgroundImage: `url(${ClosetBackground})` }}
    >
      <DressingRoom />
    </div>
  )}
</div>

); }

// COMPONENTS/ChatBox.js /* import React from 'react';

export default function ChatBox() { return ( <div className="flex flex-col h-full"> <div className="p-2 bg-gray-100 text-xs font-bold text-gray-600"> 🧠 Co-Pilot is here to guide you </div> <div className="flex-1 p-2 overflow-y-auto"> <p className="text-gray-700 text-sm"> Welcome back, Megan. What would you like to do today? </p> </div> <div className="p-2"> <input
type="text"
placeholder="Type your request here..."
className="w-full border px-2 py-1 rounded focus:outline-none text-sm"
/> </div> </div> ); } */

// COMPONENTS/DressingRoom.js /* import React from 'react';

export default function DressingRoom() { return ( <div className="w-full h-full bg-white bg-opacity-70 p-4 overflow-auto"> <h2 className="text-xl font-bold mb-2">👕 PPE & Uniform Setup</h2>

<p className="mb-2">Please confirm your uniform sizes:</p>
  <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
    <input className="border p-2" placeholder="Shirt Size" />
    <input className="border p-2" placeholder="Pants Size" />
    <input className="border p-2" placeholder="Shoe Size (Steel-Toe)" />
  </div>

  <p className="mt-4">🦺 Required PPE:</p>
  <ul className="list-disc pl-6 text-sm">
    <li>High-visibility vest</li>
    <li>Steel-toe boots</li>
    <li>Gloves (heat-resistant)</li>
    <li>Safety goggles</li>
  </ul>

  <div className="mt-4">
    <p>Do you already own this gear?</p>
    <button className="mr-2 mt-2 px-4 py-1 bg-green-600 text-white rounded">✔️ I Have It All</button>
    <a
      href="https://www.amazon.com/shop/anystaffsolutions"
      target="_blank"
      rel="noopener noreferrer"
      className="mt-2 inline-block px-4 py-1 bg-blue-600 text-white rounded"
    >
      🛒 Shop PPE (Amazon Affiliate)
    </a>
  </div>

  <div className="mt-6">
    <h3 className="text-lg font-semibold">🎨 Uniform Design Option</h3>
    <p className="text-sm text-gray-600">
      Create your own AnyStaffSolutions design. Keep it clean, respectful, and aligned with our brand values.
    </p>
    <input className="mt-2 w-full border p-2" placeholder="Describe your logo or slogan..." />
    <button className="mt-2 px-4 py-1 bg-purple-600 text-white rounded">Submit Design</button>
  </div>
</div>

); } */


