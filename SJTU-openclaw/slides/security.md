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
        Put every agent workspace under <strong>version control</strong>
      </div>
      <div class="flex items-start gap-3" style="font-size: 15px; line-height: 1.5;">
        <span style="color: rgba(0,229,255,0.6); flex-shrink: 0; font-size: 18px; margin-top: 1px;">·</span>
        Easy rollback when the agent takes a wrong turn
      </div>
      <div class="flex items-start gap-3" style="font-size: 15px; line-height: 1.5;">
        <span style="color: rgba(0,229,255,0.6); flex-shrink: 0; font-size: 18px; margin-top: 1px;">·</span>
        Audit trail: <code style="background: rgba(255,255,255,0.08); padding: 1px 5px; border-radius: 4px; font-size: 13px;">git log</code> shows exactly what changed
      </div>
      <div class="flex items-start gap-3" style="font-size: 15px; line-height: 1.5;">
        <span style="color: rgba(0,229,255,0.6); flex-shrink: 0; font-size: 18px; margin-top: 1px;">·</span>
        Enables safe experimentation — branch freely
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
        <span>Grant <strong>allow all dangerous permissions</strong> only after understanding the scope</span>
      </div>
      <div class="flex items-start gap-3" style="font-size: 15px; line-height: 1.5;">
        <span style="color: rgba(255,61,242,0.6); flex-shrink: 0; font-size: 18px; margin-top: 1px;">·</span>
        Reduces friction for trusted, well-scoped tasks
      </div>
      <div class="flex items-start gap-3" style="font-size: 15px; line-height: 1.5;">
        <span style="color: rgba(255,61,242,0.6); flex-shrink: 0; font-size: 18px; margin-top: 1px;">·</span>
        <span>Read the permission before clicking <em>yes</em> — know what you're authorizing</span>
      </div>
      <div class="flex items-start gap-3" style="font-size: 15px; line-height: 1.5;">
        <span style="color: rgba(255,61,242,0.6); flex-shrink: 0; font-size: 18px; margin-top: 1px;">·</span>
        Prefer scoped permissions per project, not global blanket allow
      </div>
    </div>
  </div>

</div>

<div v-click class="glass rounded-xl px-5 py-3 mt-6"
     style="border-left: 3px solid rgba(251,191,36,0.6); max-width: 680px;">
  <div style="display: flex; align-items: center; gap: 10px;">
    <div class="i-carbon:warning-alt" style="font-size: 20px; color: rgb(251,191,36); flex-shrink: 0;" />
    <span style="font-size: 15px; color: rgba(255,255,255,0.8);">
      <strong style="color: rgb(251,191,36);">Trust + verify</strong> — code review is still your responsibility,
      even when the agent wrote it.
    </span>
  </div>
</div>
