---
clicks: 2
transition: fade
---

# Bonus: CERN OAuth2 Mailbox

<div class="grid grid-cols-2 gap-6 mt-6">

  <!-- Left: problem + solution -->
  <div style="display: flex; flex-direction: column; gap: 16px;">
    <div class="glass rounded-xl px-5 py-4" style="border-left: 3px solid rgba(255,61,242,0.5);">
      <div style="font-size: 14px; color: rgba(255,61,242,0.8); font-weight: 600; margin-bottom: 6px; text-transform: uppercase; letter-spacing: 0.05em;">Problem</div>
      <div style="font-size: 16px; line-height: 1.55;">
        CERN email (and many institutional mailboxes) use <span style="color: #ff3df2; font-weight: 600;">OAuth2</span> —
        agents cannot authenticate natively without a configured token flow.
      </div>
    </div>
    <div v-click class="glass rounded-xl px-5 py-4" style="border-left: 3px solid rgba(0,229,255,0.5);">
      <div style="font-size: 14px; color: rgba(0,229,255,0.8); font-weight: 600; margin-bottom: 6px; text-transform: uppercase; letter-spacing: 0.05em;">Solution</div>
      <a href="https://github.com/HEPSkills/email_oauth2" target="_blank"
         style="display: flex; align-items: center; gap: 8px; text-decoration: none; margin-bottom: 10px;">
        <span class="i-ri:github-fill" style="font-size: 18px; color: #00e5ff;"></span>
        <span style="color: #00e5ff; font-size: 15px; font-weight: 600;">HEPSkills/email_oauth2</span>
      </a>
      <div style="font-size: 15px; line-height: 1.55; color: rgba(255,255,255,0.8);">
        A plug-and-play OAuth2 bridge with an <code style="background: rgba(255,255,255,0.08); padding: 1px 5px; border-radius: 4px; font-size: 13px;">OPENCLAW.md</code> that teaches the agent to self-configure.
      </div>
    </div>
    <div v-click class="glass glow-border rounded-xl px-5 py-4">
      <div style="font-size: 14px; color: rgba(0,229,255,0.7); font-style: italic; line-height: 1.5;">
        Agent self-configures OAuth2 credentials — no manual token setup needed after installation.
      </div>
    </div>
  </div>

  <!-- Right: installation -->
  <div v-click style="display: flex; flex-direction: column; gap: 14px;">
    <div style="font-size: 14px; color: rgba(255,255,255,0.55); text-transform: uppercase; letter-spacing: 0.06em; font-weight: 600;">
      How to install
    </div>
    <div class="glass rounded-xl px-5 py-4" style="border-left: 3px solid rgba(124,92,255,0.5);">
      <div style="font-size: 14px; color: rgba(255,255,255,0.5); margin-bottom: 8px; font-style: italic;">Ask your agent to:</div>
      <div style="font-family: monospace; font-size: 14px; line-height: 1.7; color: rgba(255,255,255,0.88); white-space: pre-wrap; margin: 0;">Clone this repo into<br><span style="color: #00e5ff;">~/.openclaw/workspace</span><br><br>and read<br><span style="color: #7c5cff;">~/.openclaw/workspace/email_oauth2/OPENCLAW.md</span></div>
    </div>
    <div style="font-size: 13px; color: rgba(255,255,255,0.4); font-style: italic; line-height: 1.5;">
      The OPENCLAW.md acts as a skill definition — the agent learns the tool by reading its own documentation.
    </div>
  </div>
</div>
