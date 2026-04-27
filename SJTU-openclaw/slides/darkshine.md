---
clicks: 2
transition: fade-out
---

# Scenario 1: DarkSHINE Simulation

<div class="grid grid-cols-2 gap-6 mt-4" style="height: calc(100% - 100px);">
  <div style="display: flex; flex-direction: column; gap: 12px;">
    <div class="glass rounded-xl px-4 py-3" style="display: flex; flex-wrap: wrap; gap: 8px; align-items: center;">
      <div style="background: rgba(0,229,255,0.1); border: 1px solid rgba(0,229,255,0.3); border-radius: 6px; padding: 3px 10px; font-size: 13px; font-family: monospace;">
        <span style="color: rgba(255,255,255,0.5);">harness</span>
        <span style="color: #00e5ff; margin-left: 6px;">openclaw 2026.3.8</span>
      </div>
      <div style="background: rgba(124,92,255,0.1); border: 1px solid rgba(124,92,255,0.3); border-radius: 6px; padding: 3px 10px; font-size: 13px; font-family: monospace;">
        <span style="color: rgba(255,255,255,0.5);">model</span>
        <span style="color: #7c5cff; margin-left: 6px;">gemini-2.5-flash</span>
      </div>
      <a href="https://github.com/HEPSkills/darkshine-simu" target="_blank" style="background: rgba(255,255,255,0.06); border: 1px solid rgba(255,255,255,0.15); border-radius: 6px; padding: 3px 10px; font-size: 13px; color: #00e5ff; text-decoration: none; display: flex; align-items: center; gap: 5px;">
        <span class="i-ri:github-fill" style="font-size: 14px; display: inline-block;"></span> HEPSkills/darkshine-simu
      </a>
    </div>
    <div v-click="2" style="flex: 1; min-height: 0; border-radius: 12px; overflow: hidden; background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); display: flex; align-items: center; justify-content: center; padding: 8px;">
      <img src="/images/dsimu_recoil_E.png" style="max-width: 65%; max-height: 100%; object-fit: contain;" />
    </div>
    <div v-click="2" style="font-size: 12px; color: rgba(255,255,255,0.45); text-align: center; margin-top: -4px">
      Recoil electron energy distribution — agent-generated output
    </div>
  </div>
  <div v-click="1" style="display: flex; flex-direction: column; min-height: 0;">
    <div style="position: relative; border-radius: 12px; overflow: hidden; background: rgba(0,0,0,0.3); flex: 1; min-height: 0; display: flex; align-items: center; justify-content: center;">
      <img src="/images/chat_dsimu_signal.png" style="height: 100%; width: auto; object-fit: contain; display: block;" />
      <div style="position: absolute; bottom: 0; left: 0; right: 0; background: linear-gradient(transparent, rgba(11,15,25,0.9)); padding: 6px 10px;">
        <span style="font-size: 11px; color: rgba(255,255,255,0.55);">Chat — signal sample production request</span>
      </div>
    </div>
  </div>
</div>
