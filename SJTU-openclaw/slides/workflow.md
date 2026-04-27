---
clicks: 9
transition: fade-out
---

# From Question to Output

<div style="margin-top: 28px; display: flex; flex-direction: column; gap: 32px;">
  <div>
    <div :class="[$clicks >= 1 ? 'opacity-100' : 'opacity-0']" class="transition duration-400"
         style="font-size: 13px; text-transform: uppercase; letter-spacing: 0.08em; color: rgba(0,229,255,0.7); margin-bottom: 10px; font-weight: 600;">
      Traditional — Script-centric
    </div>
    <div style="display: flex; align-items: center; gap: 8px; flex-wrap: wrap; font-size: 14px;">
      <div :class="[$clicks >= 1 ? 'opacity-100 scale-100' : 'opacity-0 scale-95']"
           class="transition duration-400 glass rounded-lg px-3 py-2"
           style="border-color: rgba(0,229,255,0.25); white-space: nowrap;">
        <span style="color: rgba(255,255,255,0.5); font-size: 11px; display: block; margin-bottom: 2px;">start</span>
        Question
      </div>
      <div :class="[$clicks >= 1 ? 'opacity-100' : 'opacity-0']" class="transition duration-400 delay-100" style="display: flex; flex-direction: column; align-items: center; gap: 2px;">
        <div style="font-size: 10px; color: rgba(0,229,255,0.55);">Human</div>
        <div class="arrow-anim" style="color: rgba(0,229,255,0.6); font-size: 18px; animation-delay: 0s;">→</div>
      </div>
      <div :class="[$clicks >= 2 ? 'opacity-100 scale-100' : 'opacity-0 scale-95']"
           class="transition duration-500 glass rounded-lg px-3 py-2"
           style="border-color: rgba(0,229,255,0.25); white-space: nowrap;">
        <span style="color: rgba(255,255,255,0.5); font-size: 11px; display: block; margin-bottom: 2px;">write</span>
        Script
      </div>
      <div :class="[$clicks >= 2 ? 'opacity-100' : 'opacity-0']" class="transition duration-500 delay-100">
        <div class="arrow-anim" style="color: rgba(0,229,255,0.6); font-size: 18px; animation-delay: 0.45s;">→</div>
      </div>
      <div :class="[$clicks >= 2 ? 'opacity-100 scale-100' : 'opacity-0 scale-95']"
           class="transition duration-500 delay-200 glass rounded-lg px-3 py-2"
           style="border-color: rgba(0,229,255,0.25); white-space: nowrap;">
        <span style="color: rgba(255,255,255,0.5); font-size: 11px; display: block; margin-bottom: 2px;">run</span>
        Output
      </div>
      <div :class="[$clicks >= 3 ? 'opacity-100' : 'opacity-0']" class="transition duration-500" style="display: flex; flex-direction: column; align-items: center; gap: 2px;">
        <div style="font-size: 10px; color: rgba(0,229,255,0.55);">Review+Debug</div>
        <div class="arrow-anim" style="color: rgba(0,229,255,0.6); font-size: 18px; animation-delay: 0.9s;">→</div>
      </div>
      <div :class="[$clicks >= 3 ? 'opacity-100 scale-100' : 'opacity-0 scale-95']"
           class="transition duration-500 delay-100 glass rounded-lg px-3 py-2"
           style="border-color: rgba(0,229,255,0.25); white-space: nowrap;">
        Script'
      </div>
      <div :class="[$clicks >= 3 ? 'opacity-100' : 'opacity-0']" class="transition duration-500 delay-200">
        <div class="arrow-anim" style="color: rgba(0,229,255,0.6); font-size: 18px; animation-delay: 1.35s;">→</div>
      </div>
      <div :class="[$clicks >= 3 ? 'opacity-100 scale-100' : 'opacity-0 scale-95']"
           class="transition duration-500 delay-300 glass rounded-lg px-3 py-2"
           style="border-color: rgba(0,229,255,0.25); white-space: nowrap;">
        Output'
      </div>
      <div :class="[$clicks >= 3 ? 'opacity-100' : 'opacity-0']" class="transition duration-500 delay-300 muted" style="font-size: 18px;">
        ···
      </div>
      <div :class="[$clicks >= 4 ? 'opacity-100' : 'opacity-0']" class="transition duration-500 delay-400" style="display: flex; flex-direction: column; align-items: center; gap: 2px;">
        <div style="font-size: 10px; color: rgba(0,229,255,0.55);">Human</div>
        <div class="arrow-anim" style="color: rgba(0,229,255,0.6); font-size: 18px; animation-delay: 1.8s;">→</div>
      </div>
      <div :class="[$clicks >= 4 ? 'opacity-100 scale-100' : 'opacity-0 scale-95']"
           class="transition duration-500 delay-500 glass rounded-lg px-3 py-2"
           style="border: 1px solid rgba(0,229,255,0.4); white-space: nowrap;">
        <span style="color: rgba(255,255,255,0.5); font-size: 11px; display: block; margin-bottom: 2px;">end</span>
        Document
      </div>
    </div>
  </div>
  <div :class="[$clicks >= 5 ? 'opacity-100' : 'opacity-0']" class="transition duration-500 neon-hr" style="max-width: 860px;"></div>
  <div>
    <div :class="[$clicks >= 5 ? 'opacity-100' : 'opacity-0']" class="transition duration-400"
         style="font-size: 13px; text-transform: uppercase; letter-spacing: 0.08em; color: rgba(255,61,242,0.8); margin-bottom: 10px; font-weight: 600;">
      Agentic — Skill-based
    </div>
    <div style="display: flex; align-items: center; gap: 8px; flex-wrap: wrap; font-size: 14px;">
      <div :class="[$clicks >= 5 ? 'opacity-100 scale-100' : 'opacity-0 scale-95']"
           class="transition duration-400 glass rounded-lg px-3 py-2"
           style="border-color: rgba(255,61,242,0.25); white-space: nowrap;">
        <span style="color: rgba(255,255,255,0.5); font-size: 11px; display: block; margin-bottom: 2px;">start</span>
        Question
      </div>
      <div :class="[$clicks >= 5 ? 'opacity-100' : 'opacity-0']" class="transition duration-400 delay-100" style="display: flex; flex-direction: column; align-items: center; gap: 2px;">
        <div style="font-size: 10px; color: rgba(255,61,242,0.65);">Human</div>
        <div class="arrow-anim" style="color: rgba(255,61,242,0.7); font-size: 18px; animation-delay: 0s;">→</div>
      </div>
      <div :class="[$clicks >= 6 ? 'opacity-100 scale-100' : 'opacity-0 scale-95']"
           class="transition duration-500 glass rounded-lg px-3 py-2"
           style="border-color: rgba(255,61,242,0.3); white-space: nowrap;">
        <span style="color: rgba(255,255,255,0.5); font-size: 11px; display: block; margin-bottom: 2px;">craft</span>
        MWE + Simple Document
        <span style="font-size: 11px; color: rgba(255,255,255,0.4); display: block;">(what to do & how to test)</span>
      </div>
      <div :class="[$clicks >= 7 ? 'opacity-100' : 'opacity-0']" class="transition duration-500" style="display: flex; flex-direction: column; align-items: center; gap: 2px;">
        <div style="font-size: 10px; color: rgba(255,61,242,0.65);">Agent+Human</div>
        <div class="arrow-anim" style="color: rgba(255,61,242,0.7); font-size: 18px; animation-delay: 0.9s;">→</div>
      </div>
      <div :class="[$clicks >= 7 ? 'opacity-100 scale-100' : 'opacity-0 scale-95']"
           class="transition duration-500 delay-100 glass rounded-lg px-3 py-2 pulse-glow"
           style="border-color: rgba(124,92,255,0.5); white-space: nowrap;">
        <span style="color: rgba(255,255,255,0.5); font-size: 11px; display: block; margin-bottom: 2px;">reusable</span>
        <span style="color: #7c5cff; font-weight: 600;">Skill</span>
      </div>
      <div :class="[$clicks >= 8 ? 'opacity-100' : 'opacity-0']" class="transition duration-500 delay-100">
        <div class="arrow-anim" style="color: rgba(124,92,255,0.7); font-size: 18px; animation-delay: 1.35s;">→</div>
      </div>
      <div :class="[$clicks >= 8 ? 'opacity-100 scale-100' : 'opacity-0 scale-95']"
           class="transition duration-500 delay-200 glass rounded-lg px-3 py-2"
           style="border: 1px solid rgba(124,92,255,0.45); white-space: nowrap;">
        <span style="color: rgba(255,255,255,0.5); font-size: 11px; display: block; margin-bottom: 2px;">run</span>
        Agentic Loop
      </div>
      <div :class="[$clicks >= 8 ? 'opacity-100' : 'opacity-0']" class="transition duration-500 delay-300">
        <div class="arrow-anim" style="color: rgba(124,92,255,0.7); font-size: 18px; animation-delay: 1.8s;">→</div>
      </div>
      <div :class="[$clicks >= 8 ? 'opacity-100 scale-100' : 'opacity-0 scale-95']"
           class="transition duration-500 delay-400 glass rounded-lg px-3 py-2"
           style="border: 1px solid rgba(124,92,255,0.45); white-space: nowrap;">
        <span style="color: rgba(255,255,255,0.5); font-size: 11px; display: block; margin-bottom: 2px;">end</span>
        Output
      </div>
    </div>
  </div>
</div>

<div :class="[$clicks >= 9 ? 'opacity-100' : 'opacity-0']" class="transition duration-500 delay-300 mt-6 glass rounded-lg px-5 py-3"
     style="max-width: 680px; border-left: 3px solid rgba(124,92,255,0.6);">
  <span style="color: rgba(255,255,255,0.55); font-size: 14px; font-style: italic;">
     Document before solving a problem. Think about what the reusable skills are.<br>Only do simple stuff, and scale it using agents.
  </span>
</div>
