---
clicks: 3
transition: fade-out
---

# Agent Security

<div class="grid grid-cols-2 gap-6 mt-8">

  <!-- Card 1: Use Git -->
  <div v-click class="glass rounded-xl overflow-hidden" style="border-color: rgba(0,229,255,0.2);">
    <div style="background: rgba(0,229,255,0.08); padding: 12px 20px; display: flex; align-items: center; gap: 10px; border-bottom: 1px solid rgba(0,229,255,0.15);">
      <div class="i-carbon:logo-github" style="font-size: 22px; color: #00e5ff;" />
      <span style="font-size: 17px; font-weight: 600; color: #00e5ff;">Use Git</span>
    </div>
    <div style="padding: 16px 20px; display: flex; flex-direction: column; gap: 10px;">
      <div class="flex items-start gap-3" style="font-size: 15px; line-height: 1.5;">
        <span style="color: rgba(0,229,255,0.6); flex-shrink: 0; font-size: 18px; margin-top: 1px;">·</span>
        Put every workspace under <strong>version control</strong>
      </div>
      <div class="flex items-start gap-3" style="font-size: 15px; line-height: 1.5;">
        <span style="color: rgba(0,229,255,0.6); flex-shrink: 0; font-size: 18px; margin-top: 1px;">·</span>
        Easy rollback when the agent takes a wrong turn
      </div>
      <div class="flex items-start gap-3" style="font-size: 15px; line-height: 1.5;">
        <span style="color: rgba(0,229,255,0.6); flex-shrink: 0; font-size: 18px; margin-top: 1px;">·</span>
        Don't add API keys in git repo
      </div>
    </div>
  </div>

  <!-- Card 2: Permissions -->
  <div v-click class="glass rounded-xl overflow-hidden" style="border-color: rgba(255,61,242,0.2);">
    <div style="background: rgba(255,61,242,0.08); padding: 12px 20px; display: flex; align-items: center; gap: 10px; border-bottom: 1px solid rgba(255,61,242,0.15);">
      <div class="i-carbon:security" style="font-size: 22px; color: #ff3df2;" />
      <span style="font-size: 17px; font-weight: 600; color: #ff3df2;">Permissions</span>
    </div>
    <div style="padding: 16px 20px; display: flex; flex-direction: column; gap: 10px;">
      <div class="flex items-start gap-3" style="font-size: 15px; line-height: 1.5;">
        <span style="color: rgba(255,61,242,0.6); flex-shrink: 0; font-size: 18px; margin-top: 1px;">·</span>
        <span>Grant <strong>allow all dangerous permissions</strong> only in sandbox</span>
      </div>
      <div class="flex items-start gap-3" style="font-size: 15px; line-height: 1.5;">
        <span style="color: rgba(255,61,242,0.6); flex-shrink: 0; font-size: 18px; margin-top: 1px;">·</span>
        <span>Prompt-based restrictions are <strong>fragile</strong> — enforce limits at the <strong>system level</strong> (OS permissions, container boundaries, allow/deny lists in config)</span>
      </div>
    </div>
  </div>

</div>

<!-- Card 3: Network Security -->
<div v-click class="glass rounded-xl overflow-hidden mt-6" style="border-color: rgba(74,222,128,0.2);">
  <div style="background: rgba(74,222,128,0.08); padding: 12px 20px; display: flex; align-items: center; gap: 10px; border-bottom: 1px solid rgba(74,222,128,0.15);">
    <div class="i-carbon:network-4" style="font-size: 22px; color: #4ade80;" />
    <span style="font-size: 17px; font-weight: 600; color: #4ade80;">Network Security</span>
  </div>
  <div style="padding: 16px 20px; display: grid; grid-template-columns: 1fr 1fr; gap: 10px;">
    <div class="flex items-start gap-3" style="font-size: 15px; line-height: 1.5;">
      <span style="color: rgba(74,222,128,0.6); flex-shrink: 0; font-size: 18px; margin-top: 1px;">·</span>
      <span>Use firewall in <strong>whitelist mode</strong> — deny by default, allow only what's needed. Close vulnerable ports: <code style="background: rgba(255,255,255,0.08); padding: 1px 5px; border-radius: 4px; font-size: 13px;">3389</code> RDP, FTP, frp control, openclaw gateway, etc.</span>
    </div>
    <div class="flex items-start gap-3" style="font-size: 15px; line-height: 1.5;">
      <span style="color: rgba(74,222,128,0.6); flex-shrink: 0; font-size: 18px; margin-top: 1px;">·</span>
      <span>Prefer encrypted overlay networks: <strong>WireGuard</strong>, <strong>Tailscale</strong> over exposed public ports</span>
    </div>
  </div>
</div>
