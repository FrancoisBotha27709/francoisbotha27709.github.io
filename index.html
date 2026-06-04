---
layout: null
---
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Bricky Brack</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <style>
@import url('https://fonts.googleapis.com/css2?family=Space+Mono:ital,wght@0,400;0,700;1,400&family=Syne:wght@400;600;800&family=Playfair+Display:wght@400;700&family=DM+Sans:wght@400;500;700&family=IBM+Plex+Mono:wght@400;700&family=Fraunces:wght@400;700&family=Outfit:wght@400;600;800&display=swap');

:root {
  --ink: #0f0f0f;
  --paper: #f5f2eb;
  --accent: #e8462a;
  --accent2: #2a6ae8;
  --ghost: #e0ddd5;
  --sidebar-w: 200px;
  --sidebar-bg: #111;
  /* global canvas vars (user-editable) */
  --canvas-bg: #f5f2eb;
  --canvas-text: #0f0f0f;
  --canvas-accent: #e8462a;
  --canvas-font: 'Syne', sans-serif;
  --canvas-mono: 'Space Mono', monospace;
}
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
html, body { width: 100%; height: 100%; }
body {
  font-family: 'Space Mono', monospace;
  background: #0a0a0a;
  color: var(--ink);
  overflow: hidden;
}

/* ── SIDEBAR ── */
#sidebar {
  position: fixed;
  top: 0; left: 0;
  width: var(--sidebar-w);
  height: 100vh;
  flex-shrink: 0;
  background: var(--sidebar-bg);
  display: flex;
  flex-direction: column;
  overflow-y: auto;
  overflow-x: hidden;
  z-index: 9999;
  border-right: 2px solid #222;
  scrollbar-width: thin;
  scrollbar-color: #333 transparent;
}
#sidebar::-webkit-scrollbar { width: 4px; }
#sidebar::-webkit-scrollbar-thumb { background: #333; border-radius: 2px; }

.sb-brand {
  font-family: 'Syne', sans-serif;
  font-weight: 800;
  font-size: 15px;
  color: #fff;
  letter-spacing: .06em;
  padding: 18px 14px 14px;
  border-bottom: 1px solid #222;
  display: flex;
  align-items: center;
  gap: 8px;
  flex-shrink: 0;
}
.sb-brand-dot { width: 8px; height: 8px; background: var(--accent); border-radius: 50%; flex-shrink: 0; }

.sb-section { padding: 10px 10px 4px; flex-shrink: 0; }
.sb-section-label {
  font-size: 8px;
  letter-spacing: .14em;
  text-transform: uppercase;
  color: #444;
  padding: 0 4px;
  margin-bottom: 4px;
  font-family: 'Space Mono', monospace;
}
.sb-btn {
  display: flex;
  align-items: center;
  gap: 8px;
  width: 100%;
  background: transparent;
  border: none;
  color: #999;
  font-family: 'Space Mono', monospace;
  font-size: 11px;
  padding: 7px 10px;
  cursor: pointer;
  border-radius: 4px;
  transition: background .12s, color .12s;
  text-align: left;
  white-space: nowrap;
}
.sb-btn:hover { background: #1e1e1e; color: #eee; }
.sb-btn.active { background: var(--accent); color: #fff; }
.sb-btn svg { flex-shrink: 0; opacity: .7; }
.sb-btn:hover svg, .sb-btn.active svg { opacity: 1; }

.sb-sep { height: 1px; background: #1e1e1e; margin: 8px 10px; }

/* danger zone */
.sb-btn.danger { color: #c44; }
.sb-btn.danger:hover { background: #2a1010; color: var(--accent); }
.sb-btn.export { color: var(--accent2); }
.sb-btn.export:hover { background: #0d1e3a; color: #6ba3ff; }

/* spacer pushes bottom items down */
.sb-flex-grow { flex: 1; }

/* ── GLOBAL SETTINGS PANEL ── */
#settings-panel {
  display: none;
  padding: 10px;
  border-top: 1px solid #222;
  flex-shrink: 0;
}
#settings-panel.open { display: block; }
.sp-label { font-size: 9px; letter-spacing: .1em; text-transform: uppercase; color: #555; margin: 10px 0 4px; }
.sp-label:first-child { margin-top: 0; }
.sp-row { display: flex; gap: 5px; align-items: center; }
.sp-select {
  flex: 1;
  background: #1a1a1a;
  border: 1px solid #333;
  color: #ccc;
  font-family: 'Space Mono', monospace;
  font-size: 10px;
  padding: 5px 6px;
  border-radius: 3px;
  outline: none;
  cursor: pointer;
}
.sp-select:focus { border-color: var(--accent2); }
.sp-color { width: 32px; height: 28px; border: 1px solid #333; border-radius: 3px; padding: 2px; background: #1a1a1a; cursor: pointer; }
.sp-apply {
  width: 100%;
  background: var(--accent2);
  color: #fff;
  border: none;
  font-family: 'Space Mono', monospace;
  font-size: 10px;
  padding: 7px;
  border-radius: 3px;
  cursor: pointer;
  margin-top: 10px;
  letter-spacing: .05em;
}
.sp-apply:hover { background: #1a5abf; }

/* ── CANVAS AREA ── */
#canvas-wrap {
  position: fixed;
  top: 0;
  left: var(--sidebar-w);
  right: 0;
  bottom: 0;
  overflow: auto;
  background: var(--canvas-bg);
}
#canvas {
  position: relative;
  min-height: 100%;
  min-width: 100%;
}
#canvas.grid-on {
  background-image: linear-gradient(to right, rgba(0,0,0,.06) 1px, transparent 1px),
                    linear-gradient(to bottom, rgba(0,0,0,.06) 1px, transparent 1px);
  background-size: 24px 24px;
}

/* ── SELECTION ACTIONS BAR ── */
#sel-bar {
  display: none;
  position: fixed;
  bottom: 20px;
  left: calc(var(--sidebar-w) + 20px);
  background: #111;
  border: 1px solid #333;
  border-radius: 6px;
  padding: 4px;
  gap: 3px;
  z-index: 9998;
  align-items: center;
  box-shadow: 0 4px 24px rgba(0,0,0,.4);
}
#sel-bar.show { display: flex; }
.sel-btn {
  display: flex; align-items: center; gap: 5px;
  background: transparent; border: none; color: #aaa;
  font-family: 'Space Mono', monospace; font-size: 10px;
  padding: 5px 10px; cursor: pointer; border-radius: 4px;
  transition: background .12s, color .12s; white-space: nowrap;
}
.sel-btn:hover { background: #222; color: #fff; }
.sel-btn.del { color: #c44; }
.sel-btn.del:hover { background: #2a1010; color: var(--accent); }
.sel-divider { width: 1px; height: 20px; background: #333; }

/* ── FREE ELEMENT SHELL ── */
.free-el {
  position: absolute;
  cursor: grab;
  user-select: none;
  outline: none;
}
.free-el.dragging { cursor: grabbing; z-index: 1000; }

/* chrome ring only when selected/hover */
.el-chrome {
  position: absolute;
  inset: -5px;
  border: 2px dashed rgba(42,106,232,.4);
  border-radius: 4px;
  pointer-events: none;
  opacity: 0;
  transition: opacity .15s;
}
.free-el:hover .el-chrome { opacity: 1; }
.free-el.selected .el-chrome { opacity: 1; border-style: solid; border-color: var(--accent); }

/* resize handle */
.resize-handle {
  position: absolute;
  bottom: -8px; right: -8px;
  width: 14px; height: 14px;
  background: var(--accent);
  border: 2px solid #fff;
  border-radius: 2px;
  cursor: se-resize;
  opacity: 0;
  transition: opacity .15s;
  pointer-events: all;
  z-index: 10;
}
.free-el.selected .resize-handle { opacity: 1; }

/* element action buttons */
.el-actions {
  position: absolute;
  top: -34px; right: -5px;
  display: flex; gap: 3px;
  opacity: 0; pointer-events: none;
  transition: opacity .15s;
}
.free-el.selected .el-actions { opacity: 1; pointer-events: all; }
.el-act-btn {
  background: #111; border: none; color: #fff;
  font-size: 10px; font-family: 'Space Mono', monospace;
  padding: 4px 7px; cursor: pointer; border-radius: 2px; white-space: nowrap;
}
.el-act-btn:hover { background: var(--accent); }

/* z-level pill */
.z-pill {
  position: absolute; top: -30px; left: -5px;
  background: #333; color: #888;
  font-size: 8px; padding: 2px 5px; border-radius: 2px;
  pointer-events: none; opacity: 0;
}
.free-el.selected .z-pill { opacity: 1; }

/* ── pointer-events fix: children need to receive events when selected ── */
.free-el > *:not(.el-chrome):not(.resize-handle):not(.el-actions):not(.z-pill) {
  pointer-events: none;
}
.free-el.selected > *:not(.el-chrome):not(.resize-handle):not(.z-pill) {
  pointer-events: auto;
}

/* ── ELEMENT STYLES ── */
.el-text {
  font-family: var(--canvas-font);
  font-size: 20px;
  font-weight: 600;
  color: var(--canvas-text);
  min-width: 80px; min-height: 28px;
  outline: none;
  padding: 4px 6px;
  line-height: 1.3;
  background: transparent;
  white-space: pre-wrap;
  word-break: break-word;
  cursor: text;
}
.el-text[contenteditable="true"],
.el-heading[contenteditable="true"],
.el-card[contenteditable="true"],
.el-list[contenteditable="true"],
.el-code[contenteditable="true"],
.el-quote[contenteditable="true"],
.el-alert-body[contenteditable="true"],
.el-toggle-label[contenteditable="true"] {
  background: rgba(42,106,232,.07);
  outline: none;
  cursor: text;
}

.el-heading {
  font-family: var(--canvas-font);
  font-weight: 800;
  color: var(--canvas-text);
  outline: none;
  padding: 4px 6px;
  background: transparent;
  white-space: pre-wrap;
  word-break: break-word;
  line-height: 1.15;
  min-width: 120px;
  cursor: text;
}
.el-heading.h1 { font-size: 48px; }
.el-heading.h2 { font-size: 32px; }
.el-heading.h3 { font-size: 22px; }

.el-list {
  font-family: var(--canvas-mono);
  font-size: 13px;
  color: var(--canvas-text);
  padding: 6px 6px 6px 24px;
  min-width: 160px;
  outline: none;
  background: transparent;
  line-height: 1.7;
  cursor: text;
}

.el-card {
  background: #fff;
  border: 2px solid var(--canvas-text);
  border-radius: 4px;
  padding: 18px 22px;
  min-width: 140px; min-height: 70px;
  box-shadow: 4px 4px 0 var(--canvas-text);
  font-family: var(--canvas-mono);
  font-size: 13px;
  white-space: pre-wrap;
  word-break: break-word;
  outline: none;
  line-height: 1.5;
  cursor: text;
}

.el-button {
  font-family: var(--canvas-mono);
  font-size: 13px; font-weight: 700;
  letter-spacing: .06em;
  padding: 10px 22px;
  background: var(--canvas-text);
  color: var(--canvas-bg);
  border: 2px solid var(--canvas-text);
  cursor: pointer; border-radius: 3px;
  transition: background .15s, color .15s;
  white-space: nowrap;
  text-decoration: none;
  display: inline-block;
}

.el-img-wrap {
  position: relative; display: block;
  min-width: 80px; min-height: 60px;
  background: var(--ghost); overflow: hidden;
}
.el-img-wrap img { width: 100%; height: 100%; object-fit: cover; display: block; pointer-events: none; }
.img-placeholder {
  position: absolute; inset: 0;
  display: flex; flex-direction: column;
  align-items: center; justify-content: center;
  gap: 6px; color: #999;
  font-size: 11px; font-family: 'Space Mono', monospace;
  pointer-events: none;
}

.el-divider { height: 3px; background: var(--canvas-text); min-width: 10px; border-radius: 2px; }

.el-video {
  position: relative; min-width: 80px; min-height: 60px;
  background: #111; overflow: hidden; display: block;
}
.el-video iframe { width: 100%; height: 100%; border: none; display: block; pointer-events: none; }
.vid-placeholder {
  position: absolute; inset: 0;
  display: flex; flex-direction: column;
  align-items: center; justify-content: center;
  gap: 8px; color: #666;
  font-size: 11px; font-family: 'Space Mono', monospace;
}

.el-icon {
  display: flex; align-items: center; justify-content: center;
  min-width: 48px; min-height: 48px;
  font-size: 48px; line-height: 1;
}

.el-code {
  font-family: var(--canvas-mono);
  font-size: 12px;
  background: #1a1a1a; color: #e0ddd5;
  border: 2px solid var(--canvas-text);
  border-radius: 3px;
  padding: 14px 16px;
  min-width: 200px; min-height: 60px;
  outline: none;
  white-space: pre; overflow-x: auto;
  line-height: 1.6;
  box-shadow: 4px 4px 0 var(--canvas-text);
  cursor: text;
}

.el-badge {
  display: inline-block;
  font-family: var(--canvas-mono);
  font-size: 11px; font-weight: 700;
  letter-spacing: .07em;
  padding: 5px 13px;
  border-radius: 999px;
  border: 2px solid currentColor;
  white-space: nowrap;
}

.el-progress-wrap { font-family: var(--canvas-mono); min-width: 160px; padding: 6px 0; }
.el-progress-label { font-size: 10px; letter-spacing: .08em; text-transform: uppercase; margin-bottom: 6px; display: flex; justify-content: space-between; color: var(--canvas-text); }
.el-progress-track { height: 10px; background: #e0ddd5; border: 2px solid var(--canvas-text); border-radius: 2px; overflow: hidden; }
.el-progress-fill { height: 100%; background: var(--canvas-accent); transition: width .3s; }

.el-spacer {
  background: repeating-linear-gradient(45deg, transparent, transparent 4px, rgba(0,0,0,.06) 4px, rgba(0,0,0,.06) 8px);
  border: 1.5px dashed #bbb; border-radius: 2px;
  min-width: 80px;
  display: flex; align-items: center; justify-content: center;
  color: #bbb; font-size: 9px; font-family: 'Space Mono', monospace;
  letter-spacing: .1em;
}

.el-quote {
  font-family: var(--canvas-font);
  font-size: 18px; font-style: italic;
  color: var(--canvas-text);
  border-left: 5px solid var(--canvas-accent);
  padding: 14px 18px;
  min-width: 200px;
  background: rgba(232,70,42,.05);
  outline: none;
  white-space: pre-wrap; word-break: break-word; line-height: 1.5;
  cursor: text;
}

.el-table-wrap { overflow: auto; min-width: 200px; }
.el-table { border-collapse: collapse; font-family: var(--canvas-mono); font-size: 12px; width: 100%; }
.el-table th { background: var(--canvas-text); color: var(--canvas-bg); padding: 7px 12px; text-align: left; font-size: 11px; letter-spacing: .06em; }
.el-table td { border: 1px solid #ddd; padding: 6px 12px; }
.el-table tr:nth-child(even) td { background: rgba(0,0,0,.03); }

.el-counter-wrap {
  font-family: var(--canvas-mono); text-align: center;
  padding: 12px 20px; background: #fff;
  border: 2px solid var(--canvas-text);
  border-radius: 4px;
  box-shadow: 4px 4px 0 var(--canvas-text);
  min-width: 120px;
}
.el-counter-num { font-family: var(--canvas-font); font-size: 48px; font-weight: 800; line-height: 1; color: var(--canvas-text); }
.el-counter-label { font-size: 10px; letter-spacing: .1em; text-transform: uppercase; color: #666; margin-top: 4px; }
.el-counter-btns { display: flex; gap: 6px; justify-content: center; margin-top: 10px; }
.el-counter-btn {
  background: var(--canvas-text); color: var(--canvas-bg);
  border: none; width: 30px; height: 30px;
  font-size: 18px; cursor: pointer; border-radius: 3px;
  font-family: var(--canvas-mono);
  display: flex; align-items: center; justify-content: center;
}
.el-counter-btn:hover { background: var(--canvas-accent); }

.el-toggle-wrap { display: flex; align-items: center; gap: 12px; font-family: var(--canvas-mono); font-size: 13px; padding: 8px; color: var(--canvas-text); }
.el-toggle-track { width: 44px; height: 24px; background: #ccc; border-radius: 12px; border: 2px solid var(--canvas-text); cursor: pointer; position: relative; transition: background .2s; flex-shrink: 0; }
.el-toggle-track.on { background: var(--canvas-accent); }
.el-toggle-thumb { position: absolute; top: 2px; left: 2px; width: 16px; height: 16px; background: #fff; border-radius: 50%; border: 1.5px solid var(--canvas-text); transition: left .2s; }
.el-toggle-track.on .el-toggle-thumb { left: 22px; }
.el-toggle-label { outline: none; min-width: 60px; cursor: text; }

.el-rating-wrap { display: flex; align-items: center; gap: 6px; font-family: var(--canvas-mono); font-size: 11px; padding: 6px; }
.el-star { font-size: 24px; cursor: pointer; line-height: 1; transition: transform .1s; user-select: none; }
.el-star:hover { transform: scale(1.2); }
.el-rating-val { font-size: 11px; color: #666; margin-left: 4px; }

.el-separator {
  display: flex; align-items: center; gap: 10px;
  min-width: 180px;
  font-family: var(--canvas-mono);
  font-size: 10px; letter-spacing: .1em; color: #999; text-transform: uppercase;
}
.el-separator::before, .el-separator::after { content: ''; flex: 1; height: 1px; background: currentColor; }

.el-colorblock { min-width: 80px; min-height: 80px; border-radius: 4px; border: 2px solid var(--canvas-text); }

.el-kbd { display: inline-flex; align-items: center; gap: 4px; font-family: var(--canvas-mono); flex-wrap: wrap; padding: 6px; }
.el-key { background: #fff; border: 1.5px solid var(--canvas-text); border-radius: 4px; box-shadow: 0 2px 0 var(--canvas-text); font-size: 12px; padding: 4px 10px; font-family: var(--canvas-mono); font-weight: 700; white-space: nowrap; }

.el-alert { display: flex; align-items: flex-start; gap: 12px; padding: 14px 16px; border-radius: 4px; border-left: 5px solid; min-width: 200px; font-family: var(--canvas-mono); font-size: 13px; line-height: 1.5; }
.el-alert.info { background: #eef3fd; border-color: var(--accent2); color: #1a3a80; }
.el-alert.warn { background: #fdfaee; border-color: #c49a1a; color: #7a5a00; }
.el-alert.error { background: #fdf0ee; border-color: var(--accent); color: #7a1a1a; }
.el-alert.ok { background: #edfdf0; border-color: #1a8c3a; color: #0d4a1e; }
.el-alert-icon { font-size: 16px; flex-shrink: 0; margin-top: 1px; }
.el-alert-body { outline: none; flex: 1; cursor: text; }

/* ── MODALS ── */
.modal-overlay {
  position: fixed; inset: 0;
  background: rgba(0,0,0,.65);
  backdrop-filter: blur(2px);
  z-index: 99999; display: flex; align-items: center; justify-content: center;
  opacity: 0; pointer-events: none; transition: opacity .2s;
}
.modal-overlay.open { opacity: 1; pointer-events: all; }
.modal {
  background: var(--paper);
  border: 2px solid var(--ink);
  box-shadow: 6px 6px 0 var(--ink);
  padding: 28px 32px;
  width: 420px; max-width: 92vw;
  border-radius: 4px;
  transform: translateY(12px) scale(.98);
  transition: transform .2s;
  font-family: 'Space Mono', monospace;
  max-height: 90vh; overflow-y: auto;
  color: var(--ink);
  position: relative;
}
.modal-overlay.open .modal { transform: translateY(0) scale(1); }
/* bold accent stripe at top */
.modal::before {
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0;
  height: 4px;
  background: var(--accent);
  border-radius: 2px 2px 0 0;
}
.modal h3 {
  font-family: 'Syne', sans-serif;
  font-size: 20px; font-weight: 800;
  margin-bottom: 20px;
  letter-spacing: .04em;
  color: var(--ink);
  line-height: 1;
}
.modal label {
  display: block;
  font-size: 9px; letter-spacing: .12em;
  text-transform: uppercase;
  margin-bottom: 5px; margin-top: 16px;
  color: #777;
  font-family: 'Space Mono', monospace;
}
.modal input, .modal select, .modal textarea {
  width: 100%;
  font-family: 'Space Mono', monospace;
  font-size: 13px;
  padding: 9px 11px;
  border: 1.5px solid #ccc;
  border-radius: 3px;
  background: #fff;
  color: var(--ink);
  outline: none;
  transition: border-color .15s, box-shadow .15s;
}
.modal input:focus, .modal select:focus, .modal textarea:focus {
  border-color: var(--accent2);
  box-shadow: 3px 3px 0 var(--accent2);
}
.modal textarea { resize: vertical; min-height: 70px; }
.modal-actions {
  display: flex; gap: 8px;
  margin-top: 24px;
  justify-content: flex-end;
  padding-top: 16px;
  border-top: 1px solid var(--ghost);
}
.m-btn {
  font-family: 'Space Mono', monospace;
  font-size: 11px; font-weight: 700; letter-spacing: .06em;
  padding: 9px 18px;
  border: 1.5px solid var(--ink);
  border-radius: 3px;
  cursor: pointer;
  background: transparent;
  color: var(--ink);
  transition: background .15s, color .15s;
  text-transform: uppercase;
}
.m-btn:hover { background: var(--ink); color: var(--paper); }
.m-btn.primary {
  background: var(--ink); color: var(--paper);
  border-color: var(--ink);
  box-shadow: 3px 3px 0 var(--accent);
}
.m-btn.primary:hover { background: var(--accent); border-color: var(--accent); box-shadow: none; }

/* ── SNACK TOAST ── */
#snack {
  position: fixed; bottom: 24px; right: 24px;
  background: #111; color: #eee;
  font-family: 'Space Mono', monospace; font-size: 11px;
  padding: 10px 18px; border-radius: 4px;
  z-index: 99999; pointer-events: none;
  transform: translateY(60px); transition: transform .25s;
  border: 1px solid #333; white-space: nowrap;
  box-shadow: 0 4px 20px rgba(0,0,0,.4);
}
#snack.show { transform: translateY(0); }

/* ── EMPTY HINT ── */
#empty-hint {
  position: absolute; top: 50%; left: 50%;
  transform: translate(-50%,-50%);
  text-align: center; pointer-events: none;
  opacity: .25; transition: opacity .4s;
  color: var(--canvas-text);
}
#empty-hint h2 { font-family: 'Syne', sans-serif; font-size: 28px; font-weight: 800; letter-spacing: .04em; line-height: 1.2; }
#empty-hint p { margin-top: 8px; font-size: 11px; letter-spacing: .06em; font-family: 'Space Mono', monospace; }
#empty-hint.hidden { opacity: 0; }
  </style>
</head>
<body>

<!-- ── MODALS ── -->

<div class="modal-overlay" id="headingModal"><div class="modal">
  <h3>Add Heading</h3>
  <label>Level</label><select id="headingLevel"><option value="h1">H1 — Large</option><option value="h2" selected>H2 — Medium</option><option value="h3">H3 — Small</option></select>
  <label>Text</label><input id="headingText" type="text" value="Your Heading Here">
  <div class="modal-actions"><button class="m-btn" onclick="closeModal('headingModal')">Cancel</button><button class="m-btn primary" onclick="confirmAddHeading()">Add</button></div>
</div></div>

<div class="modal-overlay" id="listModal"><div class="modal">
  <h3>Add List</h3>
  <label>Type</label><select id="listType"><option value="ul">Bullet</option><option value="ol">Numbered</option></select>
  <label>Items (one per line)</label><textarea id="listItems" rows="5" placeholder="Item one&#10;Item two&#10;Item three"></textarea>
  <div class="modal-actions"><button class="m-btn" onclick="closeModal('listModal')">Cancel</button><button class="m-btn primary" onclick="confirmAddList()">Add</button></div>
</div></div>

<div class="modal-overlay" id="videoModal"><div class="modal">
  <h3>Add Video</h3>
  <label>YouTube or Vimeo URL</label><input id="videoUrl" type="text" placeholder="https://www.youtube.com/watch?v=...">
  <label>Width (px)</label><input id="videoW" type="number" value="400" min="120">
  <label>Height (px)</label><input id="videoH" type="number" value="225" min="80">
  <div class="modal-actions"><button class="m-btn" onclick="closeModal('videoModal')">Cancel</button><button class="m-btn primary" onclick="confirmAddVideo()">Add</button></div>
</div></div>

<div class="modal-overlay" id="editVideoModal"><div class="modal">
  <h3>Edit Video</h3>
  <label>YouTube or Vimeo URL</label><input id="editVideoUrl" type="text">
  <div class="modal-actions"><button class="m-btn" onclick="closeModal('editVideoModal')">Cancel</button><button class="m-btn primary" onclick="confirmEditVideo()">Save</button></div>
</div></div>

<div class="modal-overlay" id="iconModal"><div class="modal">
  <h3>Add Icon / Emoji</h3>
  <label>Emoji</label><input id="iconEmoji" type="text" value="🚀" style="font-size:24px;text-align:center">
  <label>Size (px)</label><input id="iconSize" type="number" value="48" min="16" max="256">
  <div class="modal-actions"><button class="m-btn" onclick="closeModal('iconModal')">Cancel</button><button class="m-btn primary" onclick="confirmAddIcon()">Add</button></div>
</div></div>

<div class="modal-overlay" id="badgeModal"><div class="modal">
  <h3>Add Badge / Tag</h3>
  <label>Label</label><input id="badgeLabel" type="text" value="NEW">
  <label>Color</label><select id="badgeColor"><option value="dark">Dark</option><option value="red">Red</option><option value="blue">Blue</option><option value="green">Green</option><option value="yellow">Yellow</option></select>
  <div class="modal-actions"><button class="m-btn" onclick="closeModal('badgeModal')">Cancel</button><button class="m-btn primary" onclick="confirmAddBadge()">Add</button></div>
</div></div>

<div class="modal-overlay" id="progressModal"><div class="modal">
  <h3>Add Progress Bar</h3>
  <label>Label</label><input id="progressLabel" type="text" value="Progress">
  <label>Value (0–100)</label><input id="progressValue" type="number" value="65" min="0" max="100">
  <label>Width (px)</label><input id="progressWidth" type="number" value="280" min="80">
  <div class="modal-actions"><button class="m-btn" onclick="closeModal('progressModal')">Cancel</button><button class="m-btn primary" onclick="confirmAddProgress()">Add</button></div>
</div></div>

<div class="modal-overlay" id="btnModal"><div class="modal">
  <h3>Add Button</h3>
  <label>Label</label><input id="btnLabel" type="text" value="Click me">
  <label>Link URL (optional)</label><input id="btnUrl" type="text" placeholder="https://example.com">
  <label>Style</label><select id="btnStyle"><option value="dark">Dark (default)</option><option value="accent">Red accent</option><option value="blue">Blue</option><option value="outline">Outline</option><option value="ghost">Ghost</option></select>
  <label>Open in</label><select id="btnTarget"><option value="_blank">New tab</option><option value="_self">Same tab</option></select>
  <div class="modal-actions"><button class="m-btn" onclick="closeModal('btnModal')">Cancel</button><button class="m-btn primary" onclick="confirmAddButton()">Add</button></div>
</div></div>

<div class="modal-overlay" id="editBtnModal"><div class="modal">
  <h3>Edit Button</h3>
  <label>Label</label><input id="editBtnLabel" type="text">
  <label>Link URL</label><input id="editBtnUrl" type="text">
  <label>Open in</label><select id="editBtnTarget"><option value="_blank">New tab</option><option value="_self">Same tab</option></select>
  <div class="modal-actions"><button class="m-btn" onclick="closeModal('editBtnModal')">Cancel</button><button class="m-btn primary" onclick="confirmEditButton()">Save</button></div>
</div></div>

<div class="modal-overlay" id="imgModal"><div class="modal">
  <h3>Add Image</h3>
  <label>Image URL</label><input id="imgUrl" type="text" placeholder="https://example.com/photo.jpg">
  <label>— or — Upload file</label><input id="imgFile" type="file" accept="image/*">
  <label>Alt text</label><input id="imgAlt" type="text">
  <label>Link URL (optional)</label><input id="imgLink" type="text">
  <div class="modal-actions"><button class="m-btn" onclick="closeModal('imgModal')">Cancel</button><button class="m-btn primary" onclick="confirmAddImage()">Add</button></div>
</div></div>

<div class="modal-overlay" id="editImgModal"><div class="modal">
  <h3>Edit Image</h3>
  <label>Image URL</label><input id="editImgUrl" type="text">
  <label>— or — Upload new file</label><input id="editImgFile" type="file" accept="image/*">
  <label>Alt text</label><input id="editImgAlt" type="text">
  <label>Link URL</label><input id="editImgLink" type="text">
  <div class="modal-actions"><button class="m-btn" onclick="closeModal('editImgModal')">Cancel</button><button class="m-btn primary" onclick="confirmEditImage()">Save</button></div>
</div></div>

<div class="modal-overlay" id="quoteModal"><div class="modal">
  <h3>Add Quote</h3>
  <label>Quote text</label><textarea id="quoteText" rows="4" placeholder="The best way to predict the future…"></textarea>
  <label>Attribution (optional)</label><input id="quoteAttrib" type="text" placeholder="— Someone famous">
  <div class="modal-actions"><button class="m-btn" onclick="closeModal('quoteModal')">Cancel</button><button class="m-btn primary" onclick="confirmAddQuote()">Add</button></div>
</div></div>

<div class="modal-overlay" id="tableModal"><div class="modal">
  <h3>Add Table</h3>
  <label>Columns (comma-separated headers)</label><input id="tableHeaders" type="text" value="Name, Role, Status">
  <label>Rows (one per line, cells comma-separated)</label><textarea id="tableRows" rows="5" placeholder="Alice, Designer, Active&#10;Bob, Dev, Active&#10;Carol, PM, Away"></textarea>
  <div class="modal-actions"><button class="m-btn" onclick="closeModal('tableModal')">Cancel</button><button class="m-btn primary" onclick="confirmAddTable()">Add</button></div>
</div></div>

<div class="modal-overlay" id="counterModal"><div class="modal">
  <h3>Add Counter</h3>
  <label>Label</label><input id="counterLabel" type="text" value="Count">
  <label>Starting value</label><input id="counterStart" type="number" value="0">
  <div class="modal-actions"><button class="m-btn" onclick="closeModal('counterModal')">Cancel</button><button class="m-btn primary" onclick="confirmAddCounter()">Add</button></div>
</div></div>

<div class="modal-overlay" id="alertModal"><div class="modal">
  <h3>Add Alert / Callout</h3>
  <label>Type</label><select id="alertType"><option value="info">ℹ Info</option><option value="warn">⚠ Warning</option><option value="error">✕ Error</option><option value="ok">✓ Success</option></select>
  <label>Message</label><textarea id="alertText" rows="3" placeholder="Something important to note…"></textarea>
  <div class="modal-actions"><button class="m-btn" onclick="closeModal('alertModal')">Cancel</button><button class="m-btn primary" onclick="confirmAddAlert()">Add</button></div>
</div></div>

<div class="modal-overlay" id="sepModal"><div class="modal">
  <h3>Add Separator</h3>
  <label>Label (optional)</label><input id="sepLabel" type="text" placeholder="OR">
  <label>Width (px)</label><input id="sepWidth" type="number" value="300" min="80">
  <div class="modal-actions"><button class="m-btn" onclick="closeModal('sepModal')">Cancel</button><button class="m-btn primary" onclick="confirmAddSeparator()">Add</button></div>
</div></div>

<div class="modal-overlay" id="colorblockModal"><div class="modal">
  <h3>Add Color Block</h3>
  <label>Color</label><input id="colorblockColor" type="color" value="#e8462a" style="height:44px;padding:2px">
  <label>Width (px)</label><input id="colorblockW" type="number" value="120" min="20">
  <label>Height (px)</label><input id="colorblockH" type="number" value="80" min="20">
  <div class="modal-actions"><button class="m-btn" onclick="closeModal('colorblockModal')">Cancel</button><button class="m-btn primary" onclick="confirmAddColorblock()">Add</button></div>
</div></div>

<div class="modal-overlay" id="kbdModal"><div class="modal">
  <h3>Add Keyboard Shortcut</h3>
  <label>Keys (comma-separated)</label><input id="kbdKeys" type="text" value="Ctrl, S" placeholder="Ctrl, Shift, P">
  <div class="modal-actions"><button class="m-btn" onclick="closeModal('kbdModal')">Cancel</button><button class="m-btn primary" onclick="confirmAddKbd()">Add</button></div>
</div></div>

<div id="snack"></div>

<!-- ── LAYOUT ── -->
<div id="sidebar">
  <div class="sb-brand">
    <div class="sb-brand-dot"></div>
    BRICKY BRACK
  </div>

  <!-- TEXT -->
  <div class="sb-section">
    <div class="sb-section-label">Text</div>
    <button class="sb-btn" onclick="openAddHeading()">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><path d="M2 2v10M2 7h10M12 2v10" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"/></svg>Heading
    </button>
    <button class="sb-btn" onclick="addElement('text')">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><path d="M1 2h12M7 2v10M4 12h6" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"/></svg>Text
    </button>
    <button class="sb-btn" onclick="openAddList()">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><circle cx="2.5" cy="4" r="1" fill="currentColor"/><circle cx="2.5" cy="7" r="1" fill="currentColor"/><circle cx="2.5" cy="10" r="1" fill="currentColor"/><path d="M5 4h8M5 7h8M5 10h8" stroke="currentColor" stroke-width="1.3" stroke-linecap="round"/></svg>List
    </button>
    <button class="sb-btn" onclick="addElement('code')">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><path d="M4.5 3.5L1.5 7l3 3.5M9.5 3.5L12.5 7l-3 3.5" stroke="currentColor" stroke-width="1.4" stroke-linecap="round" stroke-linejoin="round"/></svg>Code
    </button>
    <button class="sb-btn" onclick="openAddQuote()">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><path d="M2 4h3v3H2V4zm0 0c0 3 1 5 3 6M7 4h3v3H7V4zm0 0c0 3 1 5 3 6" stroke="currentColor" stroke-width="1.3" stroke-linecap="round" stroke-linejoin="round"/></svg>Quote
    </button>
  </div>

  <div class="sb-sep"></div>

  <!-- MEDIA -->
  <div class="sb-section">
    <div class="sb-section-label">Media</div>
    <button class="sb-btn" onclick="openAddImage()">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><rect x="1" y="2" width="12" height="10" rx="1.5" stroke="currentColor" stroke-width="1.5"/><path d="M1 9.5l3.5-4 3 3.5L10 6l3 5.5" stroke="currentColor" stroke-width="1.3" stroke-linecap="round" stroke-linejoin="round"/></svg>Image
    </button>
    <button class="sb-btn" onclick="openAddVideo()">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><rect x="1" y="2.5" width="9" height="9" rx="1.5" stroke="currentColor" stroke-width="1.5"/><path d="M10 5.5l3-2v7l-3-2" stroke="currentColor" stroke-width="1.4" stroke-linecap="round" stroke-linejoin="round"/></svg>Video
    </button>
    <button class="sb-btn" onclick="openAddIcon()">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><circle cx="7" cy="7" r="5.5" stroke="currentColor" stroke-width="1.5"/><path d="M4.5 8.5s.8 1.5 2.5 1.5 2.5-1.5 2.5-1.5" stroke="currentColor" stroke-width="1.3" stroke-linecap="round"/><circle cx="5" cy="5.5" r=".8" fill="currentColor"/><circle cx="9" cy="5.5" r=".8" fill="currentColor"/></svg>Icon
    </button>
  </div>

  <div class="sb-sep"></div>

  <!-- COMPONENTS -->
  <div class="sb-section">
    <div class="sb-section-label">Components</div>
    <button class="sb-btn" onclick="openAddButton()">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><rect x="1" y="3.5" width="12" height="7" rx="1.5" stroke="currentColor" stroke-width="1.5"/></svg>Button
    </button>
    <button class="sb-btn" onclick="addElement('card')">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><rect x="1" y="2" width="12" height="10" rx="1.5" stroke="currentColor" stroke-width="1.5"/><path d="M3.5 5.5h7M3.5 8h4" stroke="currentColor" stroke-width="1.3" stroke-linecap="round"/></svg>Card
    </button>
    <button class="sb-btn" onclick="openAddBadge()">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><rect x="1" y="4" width="12" height="6" rx="3" stroke="currentColor" stroke-width="1.5"/></svg>Badge
    </button>
    <button class="sb-btn" onclick="openAddProgress()">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><rect x="1" y="5" width="12" height="4" rx="2" stroke="currentColor" stroke-width="1.5"/><rect x="1" y="5" width="7" height="4" rx="2" fill="currentColor"/></svg>Progress
    </button>
    <button class="sb-btn" onclick="openAddAlert()">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><path d="M7 1L13 12H1L7 1z" stroke="currentColor" stroke-width="1.4" stroke-linejoin="round"/><path d="M7 5v3M7 10v.5" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"/></svg>Alert
    </button>
    <button class="sb-btn" onclick="openAddTable()">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><rect x="1" y="2" width="12" height="10" rx="1" stroke="currentColor" stroke-width="1.4"/><path d="M1 5h12M5 5v7M9 5v7" stroke="currentColor" stroke-width="1.2" stroke-linecap="round"/></svg>Table
    </button>
    <button class="sb-btn" onclick="openAddCounter()">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><rect x="1" y="2" width="12" height="10" rx="1.5" stroke="currentColor" stroke-width="1.4"/><path d="M5 9V5M7 7h4M9 5v4" stroke="currentColor" stroke-width="1.4" stroke-linecap="round"/></svg>Counter
    </button>
    <button class="sb-btn" onclick="addElement('toggle')">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><rect x="1" y="4" width="12" height="6" rx="3" stroke="currentColor" stroke-width="1.4"/><circle cx="10" cy="7" r="2" fill="currentColor"/></svg>Toggle
    </button>
    <button class="sb-btn" onclick="addElement('rating')">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><path d="M7 1l1.5 3 3.5.5-2.5 2.5.5 3.5L7 9l-3 1.5.5-3.5L2 4.5 5.5 4z" stroke="currentColor" stroke-width="1.3" stroke-linejoin="round"/></svg>Rating
    </button>
    <button class="sb-btn" onclick="openAddKbd()">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><rect x="1" y="3" width="12" height="8" rx="1.5" stroke="currentColor" stroke-width="1.4"/><path d="M4 6h2M7 6h3M4 9h6" stroke="currentColor" stroke-width="1.2" stroke-linecap="round"/></svg>Keyboard
    </button>
  </div>

  <div class="sb-sep"></div>

  <!-- LAYOUT -->
  <div class="sb-section">
    <div class="sb-section-label">Layout</div>
    <button class="sb-btn" onclick="addElement('divider')">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><path d="M1 7h12" stroke="currentColor" stroke-width="2" stroke-linecap="round"/></svg>Divider
    </button>
    <button class="sb-btn" onclick="openAddSeparator()">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><path d="M1 7h4M9 7h4M7 7v.01" stroke="currentColor" stroke-width="1.6" stroke-linecap="round"/></svg>Separator
    </button>
    <button class="sb-btn" onclick="addElement('spacer')">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><path d="M1 2h12M1 12h12M7 4v6" stroke="currentColor" stroke-width="1.3" stroke-linecap="round"/></svg>Spacer
    </button>
    <button class="sb-btn" onclick="openAddColorblock()">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><rect x="1" y="1" width="12" height="12" rx="2" fill="currentColor" opacity=".6"/></svg>Color Block
    </button>
  </div>

  <div class="sb-sep"></div>

  <!-- VIEW -->
  <div class="sb-section">
    <div class="sb-section-label">View</div>
    <button class="sb-btn" id="gridBtn" onclick="toggleGrid()">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><path d="M1 5h12M1 9h12M5 1v12M9 1v12" stroke="currentColor" stroke-width="1.2" stroke-linecap="round"/></svg>Grid
    </button>
  </div>

  <div class="sb-sep"></div>

  <!-- GLOBAL STYLE -->
  <div class="sb-section">
    <div class="sb-section-label">Style</div>
    <button class="sb-btn" id="styleToggleBtn" onclick="toggleSettings()">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><circle cx="7" cy="7" r="5.5" stroke="currentColor" stroke-width="1.4"/><circle cx="7" cy="7" r="2" stroke="currentColor" stroke-width="1.4"/></svg>Global Theme
    </button>
  </div>

  <div id="settings-panel">
    <div class="sp-label">Background</div>
    <div class="sp-row">
      <input class="sp-color" type="color" id="sp-bg" value="#f5f2eb">
    </div>
    <div class="sp-label">Text color</div>
    <div class="sp-row">
      <input class="sp-color" type="color" id="sp-text" value="#0f0f0f">
    </div>
    <div class="sp-label">Accent color</div>
    <div class="sp-row">
      <input class="sp-color" type="color" id="sp-accent" value="#e8462a">
    </div>
    <div class="sp-label">Display font</div>
    <select class="sp-select" id="sp-font">
      <option value="'Syne', sans-serif">Syne (default)</option>
      <option value="'Playfair Display', serif">Playfair Display</option>
      <option value="'Fraunces', serif">Fraunces</option>
      <option value="'Outfit', sans-serif">Outfit</option>
      <option value="'DM Sans', sans-serif">DM Sans</option>
      <option value="'IBM Plex Mono', monospace">IBM Plex Mono</option>
    </select>
    <div class="sp-label">Mono font</div>
    <select class="sp-select" id="sp-mono">
      <option value="'Space Mono', monospace">Space Mono (default)</option>
      <option value="'IBM Plex Mono', monospace">IBM Plex Mono</option>
      <option value="'DM Sans', sans-serif">DM Sans</option>
      <option value="'Outfit', sans-serif">Outfit</option>
    </select>
    <button class="sp-apply" onclick="applyGlobalStyle()">Apply Theme</button>
  </div>

  <div class="sb-flex-grow"></div>
  <div class="sb-sep"></div>

  <!-- BOTTOM ACTIONS -->
  <div class="sb-section" style="padding-bottom:14px">
    <button class="sb-btn export" onclick="saveToFile()">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><path d="M7 1v8M4 6l3 3 3-3M2 10v2h10v-2" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg>Export HTML
    </button>
    <button class="sb-btn danger" onclick="clearAll()">
      <svg width="13" height="13" viewBox="0 0 14 14" fill="none"><path d="M2 3.5h10M5 3.5V2h4v1.5M5.5 6v5M8.5 6v5M3 3.5l.7 8h6.6l.7-8" stroke="currentColor" stroke-width="1.4" stroke-linecap="round" stroke-linejoin="round"/></svg>Clear All
    </button>
  </div>
</div>

<!-- CANVAS -->
<div id="canvas-wrap">
  <div id="canvas">
    <div id="empty-hint">
      <h2>YOUR CANVAS<br>AWAITS</h2>
      <p>← use the sidebar to add elements</p>
    </div>
  </div>
</div>

<!-- SELECTION ACTION BAR -->
<div id="sel-bar">
  <button class="sel-btn" onclick="bringForward()">
    <svg width="11" height="11" viewBox="0 0 14 14" fill="none"><path d="M7 2v10M3 6l4-4 4 4" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg>Forward
  </button>
  <button class="sel-btn" onclick="sendBackward()">
    <svg width="11" height="11" viewBox="0 0 14 14" fill="none"><path d="M7 2v10M3 10l4 4 4-4" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg>Back
  </button>
  <div class="sel-divider"></div>
  <button class="sel-btn" onclick="duplicateSelected()">
    <svg width="11" height="11" viewBox="0 0 14 14" fill="none"><rect x="4" y="4" width="9" height="9" rx="1.2" stroke="currentColor" stroke-width="1.4"/><path d="M4 10H2.5A1.5 1.5 0 011 8.5V2.5A1.5 1.5 0 012.5 1h6A1.5 1.5 0 0110 2.5V4" stroke="currentColor" stroke-width="1.4" stroke-linecap="round"/></svg>Duplicate
  </button>
  <div class="sel-divider"></div>
  <button class="sel-btn del" onclick="deleteSelected()">
    <svg width="11" height="11" viewBox="0 0 14 14" fill="none"><path d="M2 3.5h10M5 3.5V2h4v1.5M5.5 6v5M8.5 6v5M3 3.5l.7 8h6.6l.7-8" stroke="currentColor" stroke-width="1.4" stroke-linecap="round" stroke-linejoin="round"/></svg>Delete
  </button>
</div>

<script>
/* ── STATE ── */
let elCounter = 0, selected = null, editTarget = null, gridOn = false, topZ = 10;
let canvas, emptyHint, canvasWrap;

document.addEventListener('DOMContentLoaded', () => {
  canvas = document.getElementById('canvas');
  emptyHint = document.getElementById('empty-hint');
  canvasWrap = document.getElementById('canvas-wrap');
});

/* ── UTILS ── */
function snack(msg) {
  const s = document.getElementById('snack');
  s.textContent = msg; s.classList.add('show');
  clearTimeout(s._t); s._t = setTimeout(() => s.classList.remove('show'), 2200);
}
function hideEmptyHint() { emptyHint.classList.add('hidden'); }
function openModal(id)   { document.getElementById(id).classList.add('open'); }
function closeModal(id)  { document.getElementById(id).classList.remove('open'); }

/* ── SELECTION ── */
function selectEl(el) {
  if (selected && selected !== el) selected.classList.remove('selected');
  selected = el;
  if (el) { el.classList.add('selected'); showSelBar(true); }
  else     { showSelBar(false); }
}
function showSelBar(show) {
  document.getElementById('sel-bar').classList.toggle('show', show);
}

// Deselect when clicking empty canvas
document.addEventListener('DOMContentLoaded', () => {
  document.getElementById('canvas-wrap').addEventListener('mousedown', function(e) {
    if (!e.target.closest('.free-el')) selectEl(null);
  });
  document.getElementById('canvas-wrap').addEventListener('touchstart', function(e) {
    if (!e.target.closest('.free-el')) selectEl(null);
  }, { passive: true });
});

/* ── DRAGGABLE ── */
function makeDraggable(el) {
  let startX, startY, ox, oy, dragging = false;

  function onDown(e) {
    // Don't drag when clicking inside contenteditable
    if (e.target.isContentEditable) return;
    // Don't drag on buttons/interactive inner elements (counter, toggle, rating)
    if (e.target.closest('.el-counter-btn, .el-toggle-track, .el-star, .el-act-btn, .resize-handle')) return;

    const pt = e.touches ? e.touches[0] : e;
    selectEl(el);
    el.style.zIndex = ++topZ;
    startX = pt.clientX; startY = pt.clientY;
    ox = parseInt(el.style.left) || 0;
    oy = parseInt(el.style.top)  || 0;
    dragging = true;
    el.classList.add('dragging');
    e.preventDefault();
  }

  function onMove(e) {
    if (!dragging) return;
    const pt = e.touches ? e.touches[0] : e;
    el.style.left = Math.max(0, ox + pt.clientX - startX) + 'px';
    el.style.top  = Math.max(0, oy + pt.clientY - startY) + 'px';
    if (e.type === 'touchmove') e.preventDefault();
  }

  function onUp() {
    if (!dragging) return;
    dragging = false;
    el.classList.remove('dragging');
  }

  el.addEventListener('mousedown',  onDown);
  el.addEventListener('touchstart', onDown, { passive: false });
  document.addEventListener('mousemove', onMove);
  document.addEventListener('touchmove', onMove, { passive: false });
  document.addEventListener('mouseup',   onUp);
  document.addEventListener('touchend',  onUp);
}

/* ── RESIZABLE ── */
function makeResizable(wrapper, target) {
  const handle = wrapper.querySelector('.resize-handle');
  if (!handle) return;
  let startX, startY, sw, sh, active = false;

  handle.addEventListener('mousedown', e => {
    e.stopPropagation(); e.preventDefault(); active = true;
    startX = e.clientX; startY = e.clientY;
    sw = target.offsetWidth; sh = target.offsetHeight;
    selectEl(wrapper);
  });
  document.addEventListener('mousemove', e => {
    if (!active) return;
    const nw = Math.max(60, sw + e.clientX - startX);
    const nh = Math.max(30, sh + e.clientY - startY);
    target.style.width = nw + 'px';
    const noH = ['el-text','el-heading','el-list','el-button','el-badge','el-separator','el-kbd','el-toggle-wrap','el-rating-wrap'];
    if (!noH.some(c => target.classList.contains(c))) target.style.height = nh + 'px';
  });
  document.addEventListener('mouseup', () => { active = false; });
}

/* ── WRAP ELEMENT ── */
function wrapElement(inner, x, y) {
  const wrap = document.createElement('div');
  wrap.classList.add('free-el');
  wrap.dataset.id = ++elCounter;
  wrap.style.left = x + 'px'; wrap.style.top = y + 'px'; wrap.style.zIndex = ++topZ;

  const chrome = document.createElement('div'); chrome.classList.add('el-chrome');
  const resH   = document.createElement('div'); resH.classList.add('resize-handle');
  const zpill  = document.createElement('div'); zpill.classList.add('z-pill'); zpill.textContent = 'z:' + topZ;

  wrap.appendChild(chrome);
  wrap.appendChild(inner);
  wrap.appendChild(resH);
  wrap.appendChild(zpill);

  canvas.appendChild(wrap);
  makeDraggable(wrap);
  makeResizable(wrap, inner);
  selectEl(wrap);
  hideEmptyHint();
  return wrap;
}

/* ── DOUBLE CLICK EDIT ── 
   Key fix: we enable pointer-events on the element when selected
   AND we allow dblclick even when not selected (first click selects, second enables edit)
*/
function enableDoubleClickEdit(inner) {
  // Allow dblclick to bubble up to this element regardless of pointer-events state
  inner.addEventListener('dblclick', e => {
    e.stopPropagation();
    inner.setAttribute('contenteditable', 'true');
    inner.focus();
    // place cursor at end
    const range = document.createRange();
    const sel = window.getSelection();
    range.selectNodeContents(inner);
    range.collapse(false);
    sel.removeAllRanges();
    sel.addRange(range);
  });

  inner.addEventListener('blur', () => {
    inner.setAttribute('contenteditable', 'false');
  });

  // Prevent drag when clicking inside editable area
  inner.addEventListener('mousedown', e => {
    if (inner.getAttribute('contenteditable') === 'true') {
      e.stopPropagation();
    }
  });
  inner.addEventListener('touchstart', e => {
    if (inner.getAttribute('contenteditable') === 'true') {
      e.stopPropagation();
    }
  }, { passive: true });
}

/* ── ACTION HELPERS ── */
function addActionsBar(wrap, ...btns) {
  let bar = wrap.querySelector('.el-actions');
  if (!bar) { bar = document.createElement('div'); bar.classList.add('el-actions'); wrap.appendChild(bar); }
  btns.forEach(b => bar.appendChild(b));
}
function makeActionBtn(label, cb) {
  const b = document.createElement('button');
  b.classList.add('el-act-btn'); b.textContent = label;
  b.addEventListener('mousedown', e => e.stopPropagation());
  b.addEventListener('click', cb);
  return b;
}
function randPos() {
  const w = canvasWrap ? canvasWrap.clientWidth  : window.innerWidth  - 200;
  const h = canvasWrap ? canvasWrap.clientHeight : window.innerHeight;
  return {
    x: Math.floor(Math.random() * Math.max(w - 280, 60) + 30),
    y: Math.floor(Math.random() * Math.max(h - 220, 60) + 30)
  };
}

/* ── KEYBOARD ── */
document.addEventListener('keydown', e => {
  if (!selected) return;
  if (document.activeElement && document.activeElement.isContentEditable) return;
  if (e.key === 'Delete' || e.key === 'Backspace') {
    if (document.activeElement === document.body || document.activeElement === canvasWrap || document.activeElement === canvas) deleteSelected();
  }
  const step = e.shiftKey ? 10 : 2;
  if (e.key === 'ArrowLeft')  { e.preventDefault(); selected.style.left = (parseInt(selected.style.left) - step) + 'px'; }
  if (e.key === 'ArrowRight') { e.preventDefault(); selected.style.left = (parseInt(selected.style.left) + step) + 'px'; }
  if (e.key === 'ArrowUp')    { e.preventDefault(); selected.style.top  = (parseInt(selected.style.top)  - step) + 'px'; }
  if (e.key === 'ArrowDown')  { e.preventDefault(); selected.style.top  = (parseInt(selected.style.top)  + step) + 'px'; }
});

/* ── GLOBAL STYLE ── */
function toggleSettings() {
  const panel = document.getElementById('settings-panel');
  const btn   = document.getElementById('styleToggleBtn');
  panel.classList.toggle('open');
  btn.classList.toggle('active', panel.classList.contains('open'));
}

function applyGlobalStyle() {
  const root = document.documentElement;
  const bg     = document.getElementById('sp-bg').value;
  const text   = document.getElementById('sp-text').value;
  const accent = document.getElementById('sp-accent').value;
  const font   = document.getElementById('sp-font').value;
  const mono   = document.getElementById('sp-mono').value;

  root.style.setProperty('--canvas-bg',     bg);
  root.style.setProperty('--canvas-text',   text);
  root.style.setProperty('--canvas-accent', accent);
  root.style.setProperty('--canvas-font',   font);
  root.style.setProperty('--canvas-mono',   mono);

  document.getElementById('canvas-wrap').style.background = bg;
  snack('Theme applied!');
}

/* ── SIMPLE ELEMENTS ── */
function addElement(type) {
  const p = randPos();
  let inner;

  if (type === 'text') {
    inner = document.createElement('div'); inner.classList.add('el-text');
    inner.setAttribute('contenteditable','false');
    inner.textContent = 'Double-click to edit';
    enableDoubleClickEdit(inner);

  } else if (type === 'card') {
    inner = document.createElement('div'); inner.classList.add('el-card');
    inner.setAttribute('contenteditable','false');
    inner.textContent = 'Double-click to edit this card.\nUse it for notes, descriptions, or any content blob.';
    enableDoubleClickEdit(inner);

  } else if (type === 'divider') {
    inner = document.createElement('div'); inner.classList.add('el-divider'); inner.style.width = '200px';

  } else if (type === 'code') {
    inner = document.createElement('pre'); inner.classList.add('el-code');
    inner.setAttribute('contenteditable','false');
    inner.textContent = '// double-click to edit\nconsole.log("hello world");';
    inner.style.width = '320px';
    enableDoubleClickEdit(inner);

  } else if (type === 'spacer') {
    inner = document.createElement('div'); inner.classList.add('el-spacer');
    inner.style.width = '200px'; inner.style.height = '60px'; inner.textContent = 'SPACER';

  } else if (type === 'toggle') {
    inner = document.createElement('div'); inner.classList.add('el-toggle-wrap');
    inner.innerHTML = `<div class="el-toggle-track" onclick="this.classList.toggle('on')"><div class="el-toggle-thumb"></div></div><span class="el-toggle-label" contenteditable="false">Toggle me</span>`;
    const label = inner.querySelector('.el-toggle-label');
    enableDoubleClickEdit(label);

  } else if (type === 'rating') {
    inner = document.createElement('div'); inner.classList.add('el-rating-wrap');
    let cur = 3;
    inner.innerHTML = '<span class="el-star">★</span><span class="el-star">★</span><span class="el-star">★</span><span class="el-star">☆</span><span class="el-star">☆</span><span class="el-rating-val">3/5</span>';
    const stars = inner.querySelectorAll('.el-star');
    const val   = inner.querySelector('.el-rating-val');
    function setRating(n) {
      cur = n;
      stars.forEach((s, i) => s.textContent = i < n ? '★' : '☆');
      val.textContent = n + '/5';
    }
    stars.forEach((s, i) => {
      s.addEventListener('click', e => { e.stopPropagation(); setRating(i + 1); });
      s.addEventListener('mousedown', e => e.stopPropagation());
    });
  }

  wrapElement(inner, p.x, p.y);
}

/* ── HEADING ── */
function openAddHeading() { document.getElementById('headingText').value = 'Your Heading Here'; document.getElementById('headingLevel').value = 'h2'; openModal('headingModal'); }
function confirmAddHeading() { const l = document.getElementById('headingLevel').value, t = document.getElementById('headingText').value.trim() || 'Heading'; closeModal('headingModal'); addHeadingEl(l, t); }
function addHeadingEl(level, text) {
  const p = randPos(), inner = document.createElement('div');
  inner.classList.add('el-heading', level); inner.setAttribute('contenteditable','false'); inner.textContent = text;
  enableDoubleClickEdit(inner);
  const wrap = wrapElement(inner, p.x, p.y);
  addActionsBar(wrap,
    makeActionBtn('H1', () => { inner.classList.remove('h1','h2','h3'); inner.classList.add('h1'); }),
    makeActionBtn('H2', () => { inner.classList.remove('h1','h2','h3'); inner.classList.add('h2'); }),
    makeActionBtn('H3', () => { inner.classList.remove('h1','h2','h3'); inner.classList.add('h3'); })
  );
}

/* ── LIST ── */
function openAddList() { document.getElementById('listItems').value = 'Item one\nItem two\nItem three'; document.getElementById('listType').value = 'ul'; openModal('listModal'); }
function confirmAddList() {
  const type = document.getElementById('listType').value;
  const items = document.getElementById('listItems').value.split('\n').map(s => s.trim()).filter(Boolean);
  closeModal('listModal'); addListEl(type, items);
}
function addListEl(type, items) {
  const p = randPos(), inner = document.createElement(type);
  inner.classList.add('el-list'); inner.setAttribute('contenteditable','false');
  items.forEach(txt => { const li = document.createElement('li'); li.textContent = txt; inner.appendChild(li); });
  enableDoubleClickEdit(inner); wrapElement(inner, p.x, p.y);
}

/* ── VIDEO ── */
function videoEmbedUrl(raw) {
  let m = raw.match(/(?:youtu\.be\/|youtube\.com\/(?:watch\?v=|embed\/|shorts\/))([A-Za-z0-9_-]{11})/);
  if (m) return 'https://www.youtube.com/embed/' + m[1];
  m = raw.match(/vimeo\.com\/(\d+)/);
  if (m) return 'https://player.vimeo.com/video/' + m[1];
  if (raw.includes('embed')) return raw;
  return null;
}
function openAddVideo() { document.getElementById('videoUrl').value = ''; document.getElementById('videoW').value = '400'; document.getElementById('videoH').value = '225'; openModal('videoModal'); }
function confirmAddVideo() { const raw = document.getElementById('videoUrl').value.trim(), w = parseInt(document.getElementById('videoW').value)||400, h = parseInt(document.getElementById('videoH').value)||225; closeModal('videoModal'); addVideoEl(raw, w, h); }
function addVideoEl(raw, w, h) {
  const p = randPos(), inner = document.createElement('div');
  inner.classList.add('el-video'); inner.style.width = w+'px'; inner.style.height = h+'px'; inner.dataset.rawUrl = raw||'';
  const embedUrl = raw ? videoEmbedUrl(raw) : null;
  if (embedUrl) { const f = document.createElement('iframe'); f.src = embedUrl; f.allow = 'accelerometer;autoplay;clipboard-write;encrypted-media;gyroscope;picture-in-picture'; f.allowFullscreen = true; inner.appendChild(f); }
  else inner.innerHTML = `<div class="vid-placeholder"><svg width="36" height="36" viewBox="0 0 24 24" fill="none"><rect x="2" y="3" width="20" height="18" rx="2" stroke="currentColor" stroke-width="1.5"/><polygon points="9,7 9,17 17,12" fill="currentColor"/></svg><span>Click Edit to add a video URL</span></div>`;
  const wrap = wrapElement(inner, p.x, p.y);
  addActionsBar(wrap, makeActionBtn('Edit', () => openEditVideo(wrap)));
}
function openEditVideo(wrap) { editTarget = wrap; document.getElementById('editVideoUrl').value = wrap.querySelector('.el-video').dataset.rawUrl || ''; openModal('editVideoModal'); }
function confirmEditVideo() {
  const raw = document.getElementById('editVideoUrl').value.trim(); closeModal('editVideoModal');
  const inner = editTarget.querySelector('.el-video'); inner.dataset.rawUrl = raw; inner.innerHTML = '';
  const embedUrl = raw ? videoEmbedUrl(raw) : null;
  if (embedUrl) { const f = document.createElement('iframe'); f.src = embedUrl; f.allow = 'accelerometer;autoplay;clipboard-write;encrypted-media;gyroscope;picture-in-picture'; f.allowFullscreen = true; inner.appendChild(f); }
  else inner.innerHTML = `<div class="vid-placeholder"><svg width="36" height="36" viewBox="0 0 24 24" fill="none"><rect x="2" y="3" width="20" height="18" rx="2" stroke="currentColor" stroke-width="1.5"/><polygon points="9,7 9,17 17,12" fill="currentColor"/></svg><span>Click Edit to add a video URL</span></div>`;
}

/* ── ICON ── */
function openAddIcon() { document.getElementById('iconEmoji').value = '🚀'; document.getElementById('iconSize').value = '48'; openModal('iconModal'); }
function confirmAddIcon() { const emoji = document.getElementById('iconEmoji').value.trim()||'⭐', size = parseInt(document.getElementById('iconSize').value)||48; closeModal('iconModal'); addIconEl(emoji, size); }
function addIconEl(emoji, size) {
  const p = randPos(), inner = document.createElement('div');
  inner.classList.add('el-icon'); inner.style.fontSize = size+'px'; inner.style.minWidth = size+'px'; inner.style.minHeight = size+'px'; inner.textContent = emoji;
  const wrap = wrapElement(inner, p.x, p.y);
  addActionsBar(wrap,
    makeActionBtn('S', () => inner.style.fontSize = '24px'),
    makeActionBtn('M', () => inner.style.fontSize = '48px'),
    makeActionBtn('L', () => inner.style.fontSize = '96px')
  );
}

/* ── BADGE ── */
const BADGE_COLORS = {
  dark:   { bg:'#0f0f0f', color:'#f5f2eb', border:'#0f0f0f' },
  red:    { bg:'#fdf0ee', color:'#e8462a', border:'#e8462a' },
  blue:   { bg:'#eef3fd', color:'#2a6ae8', border:'#2a6ae8' },
  green:  { bg:'#edfdf0', color:'#1a8c3a', border:'#1a8c3a' },
  yellow: { bg:'#fdfaee', color:'#b07d10', border:'#c49a1a' },
};
function openAddBadge() { document.getElementById('badgeLabel').value = 'NEW'; document.getElementById('badgeColor').value = 'dark'; openModal('badgeModal'); }
function confirmAddBadge() { const l = document.getElementById('badgeLabel').value.trim()||'TAG', c = document.getElementById('badgeColor').value; closeModal('badgeModal'); addBadgeEl(l, c); }
function addBadgeEl(label, colorKey) {
  const p = randPos(), inner = document.createElement('span');
  inner.classList.add('el-badge'); inner.textContent = label;
  const c = BADGE_COLORS[colorKey]||BADGE_COLORS.dark;
  inner.style.background = c.bg; inner.style.color = c.color; inner.style.borderColor = c.border;
  const wrap = wrapElement(inner, p.x, p.y);
  Object.keys(BADGE_COLORS).forEach(key => addActionsBar(wrap, makeActionBtn(key[0].toUpperCase()+key.slice(1), () => { const nc=BADGE_COLORS[key]; inner.style.background=nc.bg; inner.style.color=nc.color; inner.style.borderColor=nc.border; })));
}

/* ── PROGRESS ── */
function openAddProgress() { document.getElementById('progressLabel').value='Progress'; document.getElementById('progressValue').value='65'; document.getElementById('progressWidth').value='280'; openModal('progressModal'); }
function confirmAddProgress() { const l=document.getElementById('progressLabel').value.trim()||'Progress', v=Math.min(100,Math.max(0,parseInt(document.getElementById('progressValue').value)||0)), w=parseInt(document.getElementById('progressWidth').value)||280; closeModal('progressModal'); addProgressEl(l,v,w); }
function addProgressEl(label, value, width) {
  const p = randPos(), inner = document.createElement('div');
  inner.classList.add('el-progress-wrap'); inner.style.width = width+'px'; inner.dataset.value = value;
  inner.innerHTML = `<div class="el-progress-label"><span class="prog-name">${label}</span><span class="prog-pct">${value}%</span></div><div class="el-progress-track"><div class="el-progress-fill" style="width:${value}%"></div></div>`;
  const wrap = wrapElement(inner, p.x, p.y);
  [25,50,75,100].forEach(pct => addActionsBar(wrap, makeActionBtn(pct+'%', () => { inner.querySelector('.el-progress-fill').style.width=pct+'%'; inner.querySelector('.prog-pct').textContent=pct+'%'; inner.dataset.value=pct; })));
}

/* ── BUTTON ── */
const BTN_STYLES = {
  dark:    { bg:'var(--canvas-text)', color:'var(--canvas-bg)', border:'var(--canvas-text)' },
  accent:  { bg:'#e8462a', color:'#fff',    border:'#e8462a' },
  blue:    { bg:'#2a6ae8', color:'#fff',    border:'#2a6ae8' },
  outline: { bg:'transparent', color:'var(--canvas-text)', border:'var(--canvas-text)' },
  ghost:   { bg:'transparent', color:'#555', border:'#ccc' },
};
function openAddButton() { document.getElementById('btnLabel').value='Click me'; document.getElementById('btnUrl').value=''; openModal('btnModal'); }
function confirmAddButton() {
  const label=document.getElementById('btnLabel').value.trim()||'Button', url=document.getElementById('btnUrl').value.trim(), target=document.getElementById('btnTarget').value, style=document.getElementById('btnStyle').value;
  closeModal('btnModal'); addButtonEl(label, url, target, style);
}
function addButtonEl(label, url, target, styleKey) {
  const p = randPos();
  const inner = url ? document.createElement('a') : document.createElement('button');
  inner.classList.add('el-button'); inner.textContent = label;
  if (url) { inner.href=url; inner.target=target||'_blank'; inner.rel='noopener'; }
  const s = BTN_STYLES[styleKey||'dark']||BTN_STYLES.dark;
  inner.style.background=s.bg; inner.style.color=s.color; inner.style.borderColor=s.border;
  const wrap = wrapElement(inner, p.x, p.y);
  addActionsBar(wrap, makeActionBtn('Edit', () => openEditButton(wrap)));
}
function openEditButton(wrap) { editTarget=wrap; const inner=wrap.querySelector('.el-button'); document.getElementById('editBtnLabel').value=inner.textContent; document.getElementById('editBtnUrl').value=inner.href||''; document.getElementById('editBtnTarget').value=inner.target||'_blank'; openModal('editBtnModal'); }
function confirmEditButton() {
  const inner=editTarget.querySelector('.el-button'), label=document.getElementById('editBtnLabel').value.trim(), url=document.getElementById('editBtnUrl').value.trim(), target=document.getElementById('editBtnTarget').value;
  inner.textContent=label||'Button';
  if (inner.tagName==='A') { inner.href=url; inner.target=target; }
  closeModal('editBtnModal');
}

/* ── IMAGE ── */
function openAddImage() { document.getElementById('imgUrl').value=''; document.getElementById('imgFile').value=''; document.getElementById('imgAlt').value=''; document.getElementById('imgLink').value=''; openModal('imgModal'); }
function confirmAddImage() {
  const url=document.getElementById('imgUrl').value.trim(), file=document.getElementById('imgFile').files[0], alt=document.getElementById('imgAlt').value.trim(), link=document.getElementById('imgLink').value.trim();
  closeModal('imgModal');
  if (file) { const r=new FileReader(); r.onload=e=>addImageEl(e.target.result,alt,link); r.readAsDataURL(file); } else addImageEl(url||'',alt,link);
}
function addImageEl(src, alt, link) {
  const p=randPos(), outer=document.createElement('div');
  outer.classList.add('el-img-wrap'); outer.style.width='240px'; outer.style.height='200px';
  if (src) { const img=document.createElement('img'); img.src=src; img.alt=alt||''; outer.appendChild(img); outer.dataset.src=src; }
  else { const ph=document.createElement('div'); ph.classList.add('img-placeholder'); ph.innerHTML='<svg width="36" height="36" viewBox="0 0 24 24" fill="none"><rect x="3" y="3" width="18" height="18" rx="2" stroke="currentColor" stroke-width="1.5"/><circle cx="8.5" cy="8.5" r="1.5" fill="currentColor"/><path d="M3 15l5-5 4 4 3-3 6 6" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg><span>Click Edit to add image</span>'; outer.appendChild(ph); }
  outer.dataset.link=link||''; outer.dataset.alt=alt||'';
  const wrap=wrapElement(outer,p.x,p.y); addActionsBar(wrap,makeActionBtn('Edit',()=>openEditImage(wrap)));
}
function openEditImage(wrap) { editTarget=wrap; const iw=wrap.querySelector('.el-img-wrap'); document.getElementById('editImgUrl').value=iw.dataset.src||''; document.getElementById('editImgFile').value=''; document.getElementById('editImgAlt').value=iw.dataset.alt||''; document.getElementById('editImgLink').value=iw.dataset.link||''; openModal('editImgModal'); }
function confirmEditImage() {
  const url=document.getElementById('editImgUrl').value.trim(), file=document.getElementById('editImgFile').files[0], alt=document.getElementById('editImgAlt').value.trim(), link=document.getElementById('editImgLink').value.trim();
  closeModal('editImgModal');
  if (file) { const r=new FileReader(); r.onload=e=>applyEditImage(e.target.result,alt,link); r.readAsDataURL(file); } else applyEditImage(url,alt,link);
}
function applyEditImage(src, alt, link) {
  const iw=editTarget.querySelector('.el-img-wrap'); iw.innerHTML=''; iw.dataset.src=src||''; iw.dataset.alt=alt||''; iw.dataset.link=link||'';
  if (src) { const img=document.createElement('img'); img.src=src; img.alt=alt||''; iw.appendChild(img); }
  else { const ph=document.createElement('div'); ph.classList.add('img-placeholder'); ph.innerHTML='<svg width="36" height="36" viewBox="0 0 24 24" fill="none"><rect x="3" y="3" width="18" height="18" rx="2" stroke="currentColor" stroke-width="1.5"/></svg><span>Click Edit to add image</span>'; iw.appendChild(ph); }
}

/* ── QUOTE ── */
function openAddQuote() { document.getElementById('quoteText').value=''; document.getElementById('quoteAttrib').value=''; openModal('quoteModal'); }
function confirmAddQuote() {
  const text=document.getElementById('quoteText').value.trim()||'Your quote here…', attrib=document.getElementById('quoteAttrib').value.trim();
  closeModal('quoteModal');
  const p=randPos(), inner=document.createElement('blockquote');
  inner.classList.add('el-quote'); inner.setAttribute('contenteditable','false');
  inner.textContent=text+(attrib?'\n— '+attrib:'');
  inner.style.width='320px';
  enableDoubleClickEdit(inner);
  wrapElement(inner,p.x,p.y);
}

/* ── TABLE ── */
function openAddTable() { document.getElementById('tableHeaders').value='Name, Role, Status'; document.getElementById('tableRows').value='Alice, Designer, Active\nBob, Dev, Active\nCarol, PM, Away'; openModal('tableModal'); }
function confirmAddTable() {
  const headers=document.getElementById('tableHeaders').value.split(',').map(s=>s.trim()).filter(Boolean);
  const rows=document.getElementById('tableRows').value.split('\n').map(r=>r.split(',').map(c=>c.trim()));
  closeModal('tableModal');
  const p=randPos(), outer=document.createElement('div'); outer.classList.add('el-table-wrap'); outer.style.width='400px';
  const tbl=document.createElement('table'); tbl.classList.add('el-table');
  const thead=document.createElement('thead'), tr=document.createElement('tr');
  headers.forEach(h=>{const th=document.createElement('th');th.textContent=h;tr.appendChild(th);});
  thead.appendChild(tr); tbl.appendChild(thead);
  const tbody=document.createElement('tbody');
  rows.forEach(row=>{const tr2=document.createElement('tr');row.forEach(cell=>{const td=document.createElement('td');td.textContent=cell;tr2.appendChild(td);});tbody.appendChild(tr2);});
  tbl.appendChild(tbody); outer.appendChild(tbl); wrapElement(outer,p.x,p.y);
}

/* ── COUNTER ── */
function openAddCounter() { document.getElementById('counterLabel').value='Count'; document.getElementById('counterStart').value='0'; openModal('counterModal'); }
function confirmAddCounter() {
  const label=document.getElementById('counterLabel').value.trim()||'Count', start=parseInt(document.getElementById('counterStart').value)||0;
  closeModal('counterModal');
  const p=randPos(), inner=document.createElement('div'); inner.classList.add('el-counter-wrap');
  inner.innerHTML=`<div class="el-counter-num">${start}</div><div class="el-counter-label">${label}</div><div class="el-counter-btns"><button class="el-counter-btn" data-d="-1">−</button><button class="el-counter-btn" data-d="1">+</button></div>`;
  const num=inner.querySelector('.el-counter-num');
  inner.querySelectorAll('.el-counter-btn').forEach(btn=>{
    btn.addEventListener('mousedown',e=>e.stopPropagation());
    btn.addEventListener('click',()=>{ num.textContent=parseInt(num.textContent)+(parseInt(btn.dataset.d)||1); });
  });
  wrapElement(inner,p.x,p.y);
}

/* ── ALERT ── */
const ALERT_ICONS = { info:'ℹ', warn:'⚠', error:'✕', ok:'✓' };
function openAddAlert() { document.getElementById('alertType').value='info'; document.getElementById('alertText').value=''; openModal('alertModal'); }
function confirmAddAlert() {
  const type=document.getElementById('alertType').value, text=document.getElementById('alertText').value.trim()||'Something to note…';
  closeModal('alertModal');
  const p=randPos(), inner=document.createElement('div'); inner.classList.add('el-alert',type);
  inner.style.width='360px';
  inner.innerHTML=`<span class="el-alert-icon">${ALERT_ICONS[type]||'ℹ'}</span><div class="el-alert-body" contenteditable="false">${text}</div>`;
  enableDoubleClickEdit(inner.querySelector('.el-alert-body'));
  const wrap=wrapElement(inner,p.x,p.y);
  addActionsBar(wrap,
    makeActionBtn('Info',()=>{inner.classList.remove('info','warn','error','ok');inner.classList.add('info');inner.querySelector('.el-alert-icon').textContent='ℹ';}),
    makeActionBtn('Warn',()=>{inner.classList.remove('info','warn','error','ok');inner.classList.add('warn');inner.querySelector('.el-alert-icon').textContent='⚠';}),
    makeActionBtn('Error',()=>{inner.classList.remove('info','warn','error','ok');inner.classList.add('error');inner.querySelector('.el-alert-icon').textContent='✕';}),
    makeActionBtn('OK',()=>{inner.classList.remove('info','warn','error','ok');inner.classList.add('ok');inner.querySelector('.el-alert-icon').textContent='✓';})
  );
}

/* ── SEPARATOR ── */
function openAddSeparator() { document.getElementById('sepLabel').value='OR'; document.getElementById('sepWidth').value='300'; openModal('sepModal'); }
function confirmAddSeparator() {
  const label=document.getElementById('sepLabel').value.trim(), width=parseInt(document.getElementById('sepWidth').value)||300;
  closeModal('sepModal');
  const p=randPos(), inner=document.createElement('div'); inner.classList.add('el-separator');
  inner.style.width=width+'px'; inner.textContent=label;
  wrapElement(inner,p.x,p.y);
}

/* ── COLOR BLOCK ── */
function openAddColorblock() { openModal('colorblockModal'); }
function confirmAddColorblock() {
  const color=document.getElementById('colorblockColor').value, w=parseInt(document.getElementById('colorblockW').value)||120, h=parseInt(document.getElementById('colorblockH').value)||80;
  closeModal('colorblockModal');
  const p=randPos(), inner=document.createElement('div'); inner.classList.add('el-colorblock');
  inner.style.width=w+'px'; inner.style.height=h+'px'; inner.style.background=color;
  const wrap=wrapElement(inner,p.x,p.y);
  addActionsBar(wrap, makeActionBtn('Color', ()=>{
    const inp=document.createElement('input'); inp.type='color'; inp.value=color;
    inp.addEventListener('input',()=>inner.style.background=inp.value);
    inp.click();
  }));
}

/* ── KEYBOARD SHORTCUT ── */
function openAddKbd() { document.getElementById('kbdKeys').value='Ctrl, S'; openModal('kbdModal'); }
function confirmAddKbd() {
  const keys=document.getElementById('kbdKeys').value.split(',').map(k=>k.trim()).filter(Boolean);
  closeModal('kbdModal');
  const p=randPos(), inner=document.createElement('div'); inner.classList.add('el-kbd');
  keys.forEach((k,i)=>{
    const span=document.createElement('span'); span.classList.add('el-key'); span.textContent=k; inner.appendChild(span);
    if(i<keys.length-1){const plus=document.createElement('span');plus.textContent='+';plus.style.color='#999';plus.style.fontSize='12px';inner.appendChild(plus);}
  });
  wrapElement(inner,p.x,p.y);
}

/* ── CANVAS ACTIONS ── */
function bringForward()  { if(selected){ selected.style.zIndex=++topZ; snack('Brought forward'); } }
function sendBackward()  { if(selected){ selected.style.zIndex=Math.max(1,(parseInt(selected.style.zIndex)||1)-2); snack('Sent backward'); } }

function duplicateSelected() {
  if (!selected) return;
  const clone = selected.cloneNode(true);
  clone.dataset.id = ++elCounter;
  clone.style.left = (parseInt(selected.style.left)+24)+'px';
  clone.style.top  = (parseInt(selected.style.top)+24)+'px';
  clone.style.zIndex = ++topZ;
  canvas.appendChild(clone);
  makeDraggable(clone);
  const inner = clone.querySelector('.el-text,.el-card,.el-img-wrap,.el-button,.el-divider,.el-heading,.el-list,.el-video,.el-icon,.el-code,.el-badge,.el-progress-wrap,.el-spacer,.el-quote,.el-table-wrap,.el-counter-wrap,.el-toggle-wrap,.el-rating-wrap,.el-separator,.el-colorblock,.el-kbd,.el-alert');
  if (inner) makeResizable(clone, inner);
  selectEl(clone); snack('Duplicated');
}

function deleteSelected() {
  if (!selected) return;
  selected.remove(); selected = null; showSelBar(false);
  if (!canvas.querySelector('.free-el')) emptyHint.classList.remove('hidden');
}

function toggleGrid() {
  gridOn = !gridOn;
  canvas.classList.toggle('grid-on', gridOn);
  document.getElementById('gridBtn').classList.toggle('active', gridOn);
}

function clearAll() {
  if (!confirm('Clear all elements? This cannot be undone.')) return;
  canvas.querySelectorAll('.free-el').forEach(e => e.remove());
  selected = null; showSelBar(false); emptyHint.classList.remove('hidden');
}

/* ── EXPORT ── */
function saveToFile() {
  const elements = [];
  canvas.querySelectorAll('.free-el').forEach(wrap => {
    const el={id:wrap.dataset.id,x:parseInt(wrap.style.left)||0,y:parseInt(wrap.style.top)||0,z:parseInt(wrap.style.zIndex)||1};
    const txt=wrap.querySelector('.el-text'),card=wrap.querySelector('.el-card'),btn=wrap.querySelector('.el-button'),imgWrap=wrap.querySelector('.el-img-wrap'),div=wrap.querySelector('.el-divider'),heading=wrap.querySelector('.el-heading'),list=wrap.querySelector('.el-list'),video=wrap.querySelector('.el-video'),icon=wrap.querySelector('.el-icon'),code=wrap.querySelector('.el-code'),badge=wrap.querySelector('.el-badge'),progress=wrap.querySelector('.el-progress-wrap'),spacer=wrap.querySelector('.el-spacer'),quote=wrap.querySelector('.el-quote'),table=wrap.querySelector('.el-table-wrap'),counter=wrap.querySelector('.el-counter-wrap'),alert_=wrap.querySelector('.el-alert'),sep=wrap.querySelector('.el-separator'),colorblock=wrap.querySelector('.el-colorblock');
    if(txt){el.type='text';el.html=txt.innerHTML;el.w=txt.style.width||'';}
    else if(card){el.type='card';el.html=card.innerHTML;el.w=card.style.width||'';}
    else if(btn){el.type='button';el.label=btn.textContent;el.url=btn.href||'';el.target=btn.target||'_blank';el.bg=btn.style.background||'';el.color=btn.style.color||'';el.border=btn.style.borderColor||'';}
    else if(imgWrap){el.type='image';el.src=imgWrap.dataset.src||'';el.alt=imgWrap.dataset.alt||'';el.link=imgWrap.dataset.link||'';el.w=imgWrap.style.width||'240px';el.h=imgWrap.style.height||'200px';}
    else if(div){el.type='divider';el.w=div.style.width||'200px';}
    else if(heading){el.type='heading';el.level=heading.classList.contains('h1')?'h1':heading.classList.contains('h3')?'h3':'h2';el.html=heading.innerHTML;el.w=heading.style.width||'';}
    else if(list){el.type='list';el.listTag=list.tagName.toLowerCase();el.html=list.innerHTML;el.w=list.style.width||'';}
    else if(video){const f=video.querySelector('iframe');el.type='video';el.rawUrl=video.dataset.rawUrl||'';el.embedUrl=f?f.src:'';el.w=video.style.width||'400px';el.h=video.style.height||'225px';}
    else if(icon){el.type='icon';el.emoji=icon.textContent;el.size=icon.style.fontSize||'48px';}
    else if(code){el.type='code';el.html=code.innerHTML;el.w=code.style.width||'';}
    else if(badge){el.type='badge';el.label=badge.textContent;el.bg=badge.style.background||'';el.color=badge.style.color||'';el.border=badge.style.borderColor||'';}
    else if(progress){const fill=progress.querySelector('.el-progress-fill'),name=progress.querySelector('.prog-name');el.type='progress';el.label=name?name.textContent:'Progress';el.value=parseInt(progress.dataset.value)||0;el.w=progress.style.width||'280px';}
    else if(spacer){el.type='spacer';el.w=spacer.style.width||'200px';el.h=spacer.style.height||'60px';}
    else if(quote){el.type='quote';el.html=quote.innerHTML;el.w=quote.style.width||'320px';}
    else if(table){el.type='table';el.html=table.innerHTML;el.w=table.style.width||'400px';}
    else if(counter){el.type='counter';el.num=counter.querySelector('.el-counter-num').textContent;el.label=counter.querySelector('.el-counter-label').textContent;}
    else if(alert_){el.type='alert';el.cls=Array.from(alert_.classList).find(c=>['info','warn','error','ok'].includes(c))||'info';el.icon=alert_.querySelector('.el-alert-icon').textContent;el.html=alert_.querySelector('.el-alert-body').innerHTML;el.w=alert_.style.width||'360px';}
    else if(sep){el.type='separator';el.label=sep.textContent;el.w=sep.style.width||'300px';}
    else if(colorblock){el.type='colorblock';el.color=colorblock.style.background||'#e8462a';el.w=colorblock.style.width||'120px';el.h=colorblock.style.height||'80px';}
    if(el.type) elements.push(el);
  });

  const root = document.documentElement;
  const style = getComputedStyle(root);
  const themeBg     = style.getPropertyValue('--canvas-bg').trim()     || '#f5f2eb';
  const themeText   = style.getPropertyValue('--canvas-text').trim()   || '#0f0f0f';
  const themeAccent = style.getPropertyValue('--canvas-accent').trim() || '#e8462a';
  const themeFont   = style.getPropertyValue('--canvas-font').trim()   || "'Syne', sans-serif";
  const themeMono   = style.getPropertyValue('--canvas-mono').trim()   || "'Space Mono', monospace";

  const html = `<!DOCTYPE html>
<html lang="en"><head><meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1.0"><title>My Page</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&family=Syne:wght@400;600;800&family=Playfair+Display:wght@400;700&family=DM+Sans:wght@400;500;700&family=IBM+Plex+Mono:wght@400;700&family=Fraunces:wght@400;700&family=Outfit:wght@400;600;800&display=swap');
:root{--canvas-bg:${themeBg};--canvas-text:${themeText};--canvas-accent:${themeAccent};--canvas-font:${themeFont};--canvas-mono:${themeMono};}
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
body{font-family:var(--canvas-mono);background:var(--canvas-bg);color:var(--canvas-text);min-height:100vh}
#page{position:relative;min-height:100vh;width:100%}.el{position:absolute}
.el-text{font-family:var(--canvas-font);font-size:20px;font-weight:600;padding:4px 6px;line-height:1.3;white-space:pre-wrap;word-break:break-word}
.el-heading{font-family:var(--canvas-font);font-weight:800;padding:4px 6px;line-height:1.15;white-space:pre-wrap;word-break:break-word}
.el-heading.h1{font-size:48px}.el-heading.h2{font-size:32px}.el-heading.h3{font-size:22px}
.el-list{font-family:var(--canvas-mono);font-size:13px;padding:6px 6px 6px 24px;line-height:1.7}
.el-card{background:#fff;border:2px solid var(--canvas-text);border-radius:4px;padding:18px 22px;box-shadow:4px 4px 0 var(--canvas-text);font-size:13px;white-space:pre-wrap;word-break:break-word;line-height:1.5}
.el-button{font-family:var(--canvas-mono);font-size:13px;font-weight:700;letter-spacing:.06em;padding:10px 22px;border:2px solid;border-radius:3px;cursor:pointer;text-decoration:none;display:inline-block}
.el-img-wrap{display:block;overflow:hidden;background:#e0ddd5}.el-img-wrap img{width:100%;height:100%;object-fit:cover;display:block}
.el-divider{height:3px;background:var(--canvas-text);border-radius:2px}
.el-video{overflow:hidden;display:block;background:#111}.el-video iframe{width:100%;height:100%;border:none;display:block}
.el-icon{display:flex;align-items:center;justify-content:center;line-height:1}
.el-code{font-family:var(--canvas-mono);font-size:12px;background:#1a1a1a;color:#e0ddd5;border:2px solid var(--canvas-text);border-radius:3px;padding:14px 16px;white-space:pre;overflow-x:auto;line-height:1.6;box-shadow:4px 4px 0 var(--canvas-text)}
.el-badge{display:inline-block;font-family:var(--canvas-mono);font-size:11px;font-weight:700;letter-spacing:.07em;padding:5px 13px;border-radius:999px;border:2px solid currentColor;white-space:nowrap}
.el-progress-wrap{font-family:var(--canvas-mono)}.el-progress-label{font-size:10px;letter-spacing:.08em;text-transform:uppercase;margin-bottom:6px;display:flex;justify-content:space-between}
.el-progress-track{height:10px;background:#e0ddd5;border:2px solid var(--canvas-text);border-radius:2px;overflow:hidden}.el-progress-fill{height:100%;background:var(--canvas-accent)}
.el-spacer{background:repeating-linear-gradient(45deg,transparent,transparent 4px,rgba(0,0,0,.06) 4px,rgba(0,0,0,.06) 8px);border:1.5px dashed #bbb;border-radius:2px}
.el-quote{font-family:var(--canvas-font);font-size:18px;font-style:italic;border-left:5px solid var(--canvas-accent);padding:14px 18px;background:rgba(232,70,42,.05);white-space:pre-wrap;word-break:break-word;line-height:1.5}
.el-table{border-collapse:collapse;font-family:var(--canvas-mono);font-size:12px;width:100%}
.el-table th{background:var(--canvas-text);color:var(--canvas-bg);padding:7px 12px;text-align:left;font-size:11px;letter-spacing:.06em}
.el-table td{border:1px solid #ddd;padding:6px 12px}.el-table tr:nth-child(even) td{background:rgba(0,0,0,.03)}
.el-counter-wrap{font-family:var(--canvas-mono);text-align:center;padding:12px 20px;background:#fff;border:2px solid var(--canvas-text);border-radius:4px;box-shadow:4px 4px 0 var(--canvas-text)}
.el-counter-num{font-family:var(--canvas-font);font-size:48px;font-weight:800;line-height:1}
.el-counter-label{font-size:10px;letter-spacing:.1em;text-transform:uppercase;color:#666;margin-top:4px}
.el-alert{display:flex;align-items:flex-start;gap:12px;padding:14px 16px;border-radius:4px;border-left:5px solid;font-family:var(--canvas-mono);font-size:13px;line-height:1.5}
.el-alert.info{background:#eef3fd;border-color:#2a6ae8;color:#1a3a80}.el-alert.warn{background:#fdfaee;border-color:#c49a1a;color:#7a5a00}
.el-alert.error{background:#fdf0ee;border-color:#e8462a;color:#7a1a1a}.el-alert.ok{background:#edfdf0;border-color:#1a8c3a;color:#0d4a1e}
.el-separator{display:flex;align-items:center;gap:10px;font-family:var(--canvas-mono);font-size:10px;letter-spacing:.1em;color:#999;text-transform:uppercase}
.el-separator::before,.el-separator::after{content:'';flex:1;height:1px;background:currentColor}
.el-colorblock{border-radius:4px;border:2px solid var(--canvas-text)}
.el-kbd{display:inline-flex;align-items:center;gap:4px;font-family:var(--canvas-mono);flex-wrap:wrap;padding:6px}
.el-key{background:#fff;border:1.5px solid var(--canvas-text);border-radius:4px;box-shadow:0 2px 0 var(--canvas-text);font-size:12px;padding:4px 10px;font-weight:700}
</style></head><body><div id="page"></div>
<script>
var E=${JSON.stringify(elements)};
(function(){var page=document.getElementById('page');E.forEach(function(el){
var w=document.createElement('div');w.className='el';w.style.left=el.x+'px';w.style.top=el.y+'px';w.style.zIndex=el.z;
if(el.type==='text'){var t=document.createElement('div');t.className='el-text';t.innerHTML=el.html;if(el.w)t.style.width=el.w;w.appendChild(t);}
else if(el.type==='heading'){var h=document.createElement('div');h.className='el-heading '+el.level;h.innerHTML=el.html;if(el.w)h.style.width=el.w;w.appendChild(h);}
else if(el.type==='list'){var l=document.createElement(el.listTag);l.className='el-list';l.innerHTML=el.html;if(el.w)l.style.width=el.w;w.appendChild(l);}
else if(el.type==='card'){var c=document.createElement('div');c.className='el-card';c.innerHTML=el.html;if(el.w)c.style.width=el.w;w.appendChild(c);}
else if(el.type==='button'){var b=el.url?document.createElement('a'):document.createElement('button');b.className='el-button';b.textContent=el.label;if(el.url){b.href=el.url;b.target=el.target;b.rel='noopener';}if(el.bg)b.style.background=el.bg;if(el.color)b.style.color=el.color;if(el.border)b.style.borderColor=el.border;w.appendChild(b);}
else if(el.type==='image'){var iw=document.createElement(el.link?'a':'div');iw.className='el-img-wrap';iw.style.width=el.w;iw.style.height=el.h;if(el.link){iw.href=el.link;iw.target='_blank';iw.rel='noopener';}if(el.src){var img=document.createElement('img');img.src=el.src;img.alt=el.alt||'';iw.appendChild(img);}w.appendChild(iw);}
else if(el.type==='divider'){var d=document.createElement('div');d.className='el-divider';d.style.width=el.w;w.appendChild(d);}
else if(el.type==='video'){var v=document.createElement('div');v.className='el-video';v.style.width=el.w;v.style.height=el.h;if(el.embedUrl){var f=document.createElement('iframe');f.src=el.embedUrl;f.allow='accelerometer;autoplay;clipboard-write;encrypted-media;gyroscope;picture-in-picture';f.allowFullscreen=true;v.appendChild(f);}w.appendChild(v);}
else if(el.type==='icon'){var ic=document.createElement('div');ic.className='el-icon';ic.style.fontSize=el.size;ic.textContent=el.emoji;w.appendChild(ic);}
else if(el.type==='code'){var pre=document.createElement('pre');pre.className='el-code';pre.innerHTML=el.html;if(el.w)pre.style.width=el.w;w.appendChild(pre);}
else if(el.type==='badge'){var bg=document.createElement('span');bg.className='el-badge';bg.textContent=el.label;if(el.bg)bg.style.background=el.bg;if(el.color)bg.style.color=el.color;if(el.border)bg.style.borderColor=el.border;w.appendChild(bg);}
else if(el.type==='progress'){var pw=document.createElement('div');pw.className='el-progress-wrap';pw.style.width=el.w;pw.innerHTML='<div class="el-progress-label"><span>'+el.label+'</span><span>'+el.value+'%</span></div><div class="el-progress-track"><div class="el-progress-fill" style="width:'+el.value+'%"></div></div>';w.appendChild(pw);}
else if(el.type==='spacer'){var sp=document.createElement('div');sp.className='el-spacer';sp.style.width=el.w;sp.style.height=el.h;w.appendChild(sp);}
else if(el.type==='quote'){var q=document.createElement('blockquote');q.className='el-quote';q.innerHTML=el.html;if(el.w)q.style.width=el.w;w.appendChild(q);}
else if(el.type==='table'){var tw=document.createElement('div');tw.className='el-table-wrap';tw.innerHTML=el.html;if(el.w)tw.style.width=el.w;w.appendChild(tw);}
else if(el.type==='counter'){var cw=document.createElement('div');cw.className='el-counter-wrap';cw.innerHTML='<div class="el-counter-num">'+el.num+'</div><div class="el-counter-label">'+el.label+'</div>';w.appendChild(cw);}
else if(el.type==='alert'){var aw=document.createElement('div');aw.className='el-alert '+el.cls;aw.style.width=el.w;aw.innerHTML='<span class="el-alert-icon">'+el.icon+'</span><div>'+el.html+'</div>';w.appendChild(aw);}
else if(el.type==='separator'){var sv=document.createElement('div');sv.className='el-separator';sv.style.width=el.w;sv.textContent=el.label;w.appendChild(sv);}
else if(el.type==='colorblock'){var cb=document.createElement('div');cb.className='el-colorblock';cb.style.background=el.color;cb.style.width=el.w;cb.style.height=el.h;w.appendChild(cb);}
page.appendChild(w);});})();
<\/script></body></html>`;

  const blob = new Blob([html], {type:'text/html'}), a = document.createElement('a');
  a.href = URL.createObjectURL(blob); a.download = 'index.html'; a.click(); snack('Exported as index.html');
}
</script>
</body>
</html>
