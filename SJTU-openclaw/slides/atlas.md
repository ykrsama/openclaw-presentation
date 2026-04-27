---
clicks: 3
transition: fade
---

# Scenario 2: ATLAS Open Data Analysis

<div class="grid grid-cols-2 gap-6 mt-6" style="height: calc(100% - 100px);">
  <div style="display: flex; flex-direction: column; gap: 14px;">
    <div class="glass rounded-xl px-5 py-4" style="border-left: 3px solid rgba(0,229,255,0.5);">
      <div style="font-size: 15px; font-weight: 600; color: #00e5ff; margin-bottom: 8px;">What the agent did</div>
      <div style="display: flex; flex-direction: column; gap: 8px; font-size: 15px; line-height: 1.5;">
        <div style="display: flex; align-items: flex-start; gap: 8px;">
          <span style="color: rgba(0,229,255,0.6); flex-shrink: 0; margin-top: 2px;">·</span>
          <span>Wrote analysis code from physics description</span>
        </div>
        <div style="display: flex; align-items: flex-start; gap: 8px;">
          <span style="color: rgba(0,229,255,0.6); flex-shrink: 0; margin-top: 2px;">·</span>
          <span>Ran over ATLAS Open Data (H&#8594;bb&#772; candidate events)</span>
        </div>
        <div style="display: flex; align-items: flex-start; gap: 8px;">
          <span style="color: rgba(0,229,255,0.6); flex-shrink: 0; margin-top: 2px;">·</span>
          <span>Produced publication-quality plots with ROOT/Python</span>
        </div>
        <div style="display: flex; align-items: flex-start; gap: 8px;">
          <span style="color: rgba(0,229,255,0.6); flex-shrink: 0; margin-top: 2px;">·</span>
          <span>Iterated on cuts and histogram binning from natural-language feedback</span>
        </div>
      </div>
    </div>
    <a v-click href="https://github.com/HEPSkills/sm-ana-aod" target="_blank" class="glass rounded-xl px-5 py-3" style="display: flex; align-items: center; gap: 10px; text-decoration: none; border-color: rgba(255,255,255,0.12);">
      <span class="i-ri:github-fill" style="font-size: 22px; color: #00e5ff; display: inline-block;"></span>
      <div>
        <div style="color: #00e5ff; font-size: 15px; font-weight: 600;">HEPSkills/sm-ana-aod</div>
        <div style="color: rgba(255,255,255,0.45); font-size: 13px; margin-top: 2px;">Analysis code + agent skill definition</div>
      </div>
    </a>
    <div v-click class="glass rounded-xl px-5 py-3" style="border-left: 3px solid rgba(124,92,255,0.45);">
      <div style="font-size: 13px; color: rgba(255,255,255,0.55); font-style: italic; line-height: 1.5;">
        Zero prior knowledge of ATLAS software stack — agent self-configured the environment and dependencies.
      </div>
    </div>
  </div>
  <div style="display: flex; flex-direction: column; gap: 10px; align-items: center; justify-content: center;">
    <div :class="[$clicks >= 3 ? 'opacity-100 scale-100' : 'opacity-0 scale-95']" class="transition duration-600" style="border-radius: 12px; overflow: hidden; background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); padding: 8px; width: 100%;">
      <img src="/images/mbb_plot.png" style="width: 100%; object-fit: contain; border-radius: 6px;" />
    </div>
    <div :class="[$clicks >= 3 ? 'opacity-100' : 'opacity-0']" class="transition duration-400" style="font-size: 12px; color: rgba(255,255,255,0.45); text-align: center;">
      m<sub>bb</sub> distribution — di-b-jet invariant mass from agent-written analysis
    </div>
  </div>
</div>
