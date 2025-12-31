import React, { useState } from 'react';

export default function PinkStardewGiftWebsite() {
  const [screen, setScreen] = useState('accept');
  const [selectedGift, setSelectedGift] = useState(null);

  const handleEnvelopeClick = () => {
    setScreen('message');
  };

  return (
    <div className="min-h-screen flex items-center justify-center p-4 relative overflow-hidden" 
         style={{
           background: 'linear-gradient(to bottom, #FFB6D9 0%, #FFC8E3 30%, #FFE5F0 60%, #FFB3D9 100%)'
         }}>
      
      {/* Pixel art style background elements */}
      <div className="absolute inset-0 pointer-events-none opacity-30">
        <div className="absolute top-10 left-10 text-4xl">🌸</div>
        <div className="absolute top-20 right-20 text-4xl">🌸</div>
        <div className="absolute bottom-20 left-20 text-3xl">🌷</div>
        <div className="absolute bottom-10 right-10 text-3xl">🌺</div>
        <div className="absolute top-1/2 left-5 text-2xl">💕</div>
        <div className="absolute top-1/3 right-10 text-2xl">🦋</div>
        <div className="absolute top-1/4 left-1/4 text-2xl">✨</div>
        <div className="absolute bottom-1/3 right-1/4 text-2xl">💫</div>
      </div>

      {/* Accept Screen */}
      {screen === 'accept' && (
        <div className="text-center animate-fade-in relative z-10">
          <div className="bg-white border-8 rounded-lg p-8 shadow-2xl max-w-lg"
               style={{
                 borderColor: '#FF69B4',
                 boxShadow: '8px 8px 0px rgba(255, 105, 180, 0.5)',
                 imageRendering: 'pixelated'
               }}>
            <h1 className="text-4xl md:text-5xl font-bold mb-8 tracking-wide"
                style={{
                  color: '#FF1493',
                  textShadow: '3px 3px 0px rgba(255, 20, 147, 0.3)',
                  fontFamily: 'monospace'
                }}>
              ACCEPT THE GIFT?
            </h1>
            
            <div className="mb-8 flex justify-center relative">
              <div className="text-7xl animate-bounce">🐰</div>
              <div className="absolute -top-2 -right-2 text-5xl animate-pulse">💗</div>
            </div>

            <div className="text-sm mb-6 text-pink-700 italic" style={{fontFamily: 'monospace'}}>
              "A mysterious gift awaits you..."
            </div>

            <div className="flex gap-4 justify-center">
              <button
                onClick={() => setScreen('gifts')}
                className="px-10 py-3 text-xl font-bold rounded shadow-lg transform transition hover:scale-105 active:scale-95 border-4"
                style={{
                  backgroundColor: '#FFB6D9',
                  color: '#C71585',
                  borderColor: '#FF69B4',
                  fontFamily: 'monospace',
                  boxShadow: '4px 4px 0px #FF69B4'
                }}
              >
                YES ✓
              </button>
              <button
                onClick={() => setScreen('refuse')}
                className="px-10 py-3 text-xl font-bold rounded shadow-lg transform transition hover:scale-105 active:scale-95 border-4"
                style={{
                  backgroundColor: '#FFC0CB',
                  color: '#8B0000',
                  borderColor: '#FF1493',
                  fontFamily: 'monospace',
                  boxShadow: '4px 4px 0px #FF1493'
                }}
              >
                NO ✗
              </button>
            </div>
          </div>
        </div>
      )}

      {/* Refuse Screen */}
      {screen === 'refuse' && (
        <div className="text-center animate-fade-in relative z-10">
          <div className="bg-white border-8 rounded-lg p-8 shadow-2xl max-w-lg"
               style={{
                 borderColor: '#FF1493',
                 boxShadow: '8px 8px 0px rgba(255, 20, 147, 0.5)'
               }}>
            <h1 className="text-4xl md:text-5xl font-bold mb-8 tracking-wide"
                style={{
                  color: '#FF1493',
                  textShadow: '3px 3px 0px rgba(255, 20, 147, 0.3)',
                  fontFamily: 'monospace'
                }}>
              FRIENDSHIP -50! 💔
            </h1>
            
            <div className="mb-8 text-7xl">
              😠🐰
            </div>

            <div className="text-sm mb-6 text-pink-700 italic" style={{fontFamily: 'monospace'}}>
              "The bunny looks disappointed..."
            </div>

            <button
              onClick={() => setScreen('accept')}
              className="px-10 py-3 text-xl font-bold rounded shadow-lg transform transition hover:scale-105 active:scale-95 border-4"
              style={{
                backgroundColor: '#FFB6D9',
                color: '#C71585',
                borderColor: '#FF69B4',
                fontFamily: 'monospace',
                boxShadow: '4px 4px 0px #FF69B4'
              }}
            >
              TRY AGAIN ↻
            </button>
          </div>
        </div>
      )}

      {/* Gifts Screen */}
      {screen === 'gifts' && (
        <div className="text-center animate-fade-in relative z-10">
          <div className="bg-white border-8 rounded-lg p-8 shadow-2xl max-w-lg"
               style={{
                 borderColor: '#FF69B4',
                 boxShadow: '8px 8px 0px rgba(255, 105, 180, 0.5)'
               }}>
            <h1 className="text-4xl md:text-5xl font-bold mb-8 tracking-wide"
                style={{
                  color: '#FF1493',
                  textShadow: '3px 3px 0px rgba(255, 20, 147, 0.3)',
                  fontFamily: 'monospace'
                }}>
              YOUR GIFT AWAITS
            </h1>
            
            <button
              onClick={handleEnvelopeClick}
              className="w-64 h-64 rounded-lg shadow-xl transform transition hover:scale-110 active:scale-95 flex flex-col items-center justify-center border-4 mx-auto"
              style={{
                backgroundColor: '#FFE4E8',
                borderColor: '#FF69B4',
                boxShadow: '6px 6px 0px #FF69B4'
              }}
            >
              <div className="text-9xl animate-bounce">💌</div>
            </button>

            <div className="flex items-center justify-center gap-2 text-pink-700 font-medium mt-8" style={{fontFamily: 'monospace'}}>
              <span>👆</span>
              <span>Click to open the envelope</span>
            </div>
          </div>
        </div>
      )}

      {/* Message Screen */}
      {screen === 'message' && (
        <div className="max-w-5xl mx-auto animate-fade-in relative z-10">
          <div className="bg-white border-8 rounded-lg shadow-2xl p-6 md:p-10"
               style={{
                 borderColor: '#FF69B4',
                 boxShadow: '8px 8px 0px rgba(255, 105, 180, 0.5)'
               }}>
            <div className="grid md:grid-cols-2 gap-8">
              
              {/* Left side - Music Box */}
              <div className="rounded-lg p-6 border-4"
                   style={{
                     background: 'linear-gradient(135deg, #FFB6D9 0%, #FF69B4 100%)',
                     borderColor: '#FF1493',
                     boxShadow: '4px 4px 0px #FF1493'
                   }}>
                <h2 className="text-2xl font-bold mb-4 text-white" style={{fontFamily: 'monospace', textShadow: '2px 2px 0px rgba(0,0,0,0.3)'}}>
                  ♪ Memory Box ♪
                </h2>
                
                <div className="rounded-lg p-6 mb-6 h-48 flex items-center justify-center border-4"
                     style={{
                       backgroundColor: '#FFE4E8',
                       borderColor: '#FF1493'
                     }}>
                  <div className="text-center">
                    <div className="text-6xl mb-2">🎵</div>
                    <div className="text-xs font-bold text-pink-700" style={{fontFamily: 'monospace'}}>
                      Flower Dance
                    </div>
                  </div>
                </div>

                <div className="space-y-3">
                  <div className="text-sm font-bold text-white" style={{fontFamily: 'monospace'}}>
                    🎼 Stardew Valley OST
                  </div>
                  <div className="flex items-center justify-center gap-4">
                    <button className="w-10 h-10 hover:bg-pink-200 rounded border-2 flex items-center justify-center transition hover:scale-110"
                            style={{
                              backgroundColor: '#FFE4E8',
                              borderColor: '#FF1493'
                            }}>
                      ⏮️
                    </button>
                    <button className="w-14 h-14 hover:bg-pink-400 rounded-full border-4 flex items-center justify-center transition hover:scale-110"
                            style={{
                              backgroundColor: '#FFB6D9',
                              borderColor: '#FF1493'
                            }}>
                      <span className="text-2xl">▶️</span>
                    </button>
                    <button className="w-10 h-10 hover:bg-pink-200 rounded border-2 flex items-center justify-center transition hover:scale-110"
                            style={{
                              backgroundColor: '#FFE4E8',
                              borderColor: '#FF1493'
                            }}>
                      ⏭️
                    </button>
                  </div>
                  <div className="text-center text-xs text-white" style={{fontFamily: 'monospace'}}>
                    ━━━━●─────── 1:23 / 3:32
                  </div>
                </div>
              </div>

              {/* Right side - Letter */}
              <div className="space-y-4 p-4 rounded-lg border-4"
                   style={{
                     backgroundColor: '#FFF0F5',
                     borderColor: '#FF69B4'
                   }}>
                <h3 className="text-xl font-bold mb-4 text-center"
                    style={{
                      color: '#FF1493',
                      fontFamily: 'monospace',
                      borderBottom: '2px solid #FF69B4',
                      paddingBottom: '8px'
                    }}>
                  💌 A Special Letter 💌
                </h3>
                
                <div className="text-sm leading-relaxed space-y-3 text-gray-800" style={{fontFamily: 'monospace'}}>
                  <p>
                    <strong style={{color: '#FF1493'}}>Dearest Noah sungit,</strong>
                  </p>
                  
                  <p>
                    Happy New Year! 🎉 Alam ko medyo late na 'to pero sige na, extension na lang ng celebration natin hehe. Gusto ko lang sabihin na sobrang special mo sa'kin. Hindi ko inexpect na magkakaroon ako ng kaibigan na katulad mo—yung tipong sobrang comfortable ako na makausap at makasama.
                  </p>

                  <p>
                    I appreciate you every single day, lalo na yung mga kwento mo sa'kin. Yung mga random rants mo, yung mga achievements mo, yung mga problema mo—lahat yan, I'm here for it. Sobrang thankful ako kasi nakilala kita. You make my days brighter, and honestly, mas masaya ang buhay ko dahil nandito ka.
                  </p>

                  <p>
                    I'm always proud of you, especially sa lahat ng achievements mo sa buhay. Yung dedication mo, yung effort mo sa lahat ng ginagawa mo—nakikita ko 'yan lahat. Sobrang inspired ako sayo, and I want you to know na you're doing amazing. Keep shining! ✨
                  </p>

                  <p>
                    Tandaan mo na nandito lang ako palagi pag kailangan mo. Kahit anong oras, kahit saan, I'll be here. Asahan mo na magrerespond ako lagi sayo—kahit busy pa ko, kahit ano pang nangyayari. You're important to me, and I hope you never forget that.
                  </p>

                  <p>
                    Cheers to more memories, more kwentuhan, more laughter, and more adventures together in 2026! Salamat sa lahat, Noah. You're one of the best things that happened to me. 💖
                  </p>

                  <p className="text-right pt-2">
                    <em>Happy New Year, Noah sungit! 🎊</em><br/><br/>
                    <strong style={{color: '#FF1493'}}>Pinakamabangs sa lahat,</strong><br/>
                    <strong style={{color: '#FF1493'}}>Polka ♡</strong>
                  </p>
                </div>

                <div className="flex justify-center gap-3 text-3xl pt-4">
                  🌸 💖 🐰 🍰 ✨
                </div>
              </div>
            </div>
          </div>
        </div>
      )}

      <style jsx>{`
        @keyframes fade-in {
          from {
            opacity: 0;
            transform: translateY(20px);
          }
          to {
            opacity: 1;
            transform: translateY(0);
          }
        }
        .animate-fade-in {
          animation: fade-in 0.5s ease-out;
        }
        @keyframes pulse {
          0%, 100% {
            opacity: 1;
            transform: scale(1);
          }
          50% {
            opacity: 0.8;
            transform: scale(1.1);
          }
        }
        .animate-pulse {
          animation: pulse 2s ease-in-out infinite;
        }
      `}</style>
    </div>
  );
}
