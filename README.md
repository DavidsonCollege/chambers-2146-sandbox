# Chambers 2146 Sandbox

An interactive 3D model of Chambers 2146, the test classroom for Davidson College's new classroom AV standard.

- Jump between camera views (room, instructor, audience, both Logi Rally cameras, reflected ceiling plan, dollhouse overview)
- Switch the displays between a presentation and a Zoom guest lecture
- Explode the Heckler 4U lectern and read about each component, with a spinning 3D model of the part
- Read the project philosophy ("Why this room")
- Try the room controller: the Q-SYS control page from Hance Auditorium, rebuilt from its UCI file. It drives the projector and motorized screen in the model, and its Cameras page shows a live view from the model's Rally cameras

Static site: `index.html` plus `model/`, `data/`, `tex/`, `img/`, `renders/` and `uci/`. three.js loads from jsDelivr. No build step.

`uci/` holds the controller: `hance.json` is the layout exported from `Hance UCI.uci` (layers, positions, CSS classes and the Core control behind each button), `sim.css` translates the Davidson UCI style sheet, and `sim.js` renders the panel and simulates the Core logic. A UCI file doesn't include the Core's Lua scripts, so that logic is inferred.

Proposed design, modeled from the room floor plan and a site photo. Product images belong to their manufacturers.
