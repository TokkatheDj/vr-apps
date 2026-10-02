# VR Math Rooms

Three small WebXR rooms for teaching on a Meta Quest, built with [A-Frame](https://aframe.io) 1.8. Each one is a single HTML file: no build step, no install.

**Open on the Quest:** https://tokkathedj.github.io/vr-apps/ in the Quest browser, pick a room, then tap **VR**.

| Room | Topic | What students do |
|---|---|---|
| Coordinate Plane | Algebra 1 | Plot points, then find the slope and the equation of a line |
| Slope Hill | Algebra 1 | Stand on y = mx + b; change m and b and feel the ground tilt; walk the line; guess mode |
| Budget Room | Personal finance | Sort a month of expenses into needs / wants / savings (50 / 30 / 20) |

Every room also works on a laptop: drag to look, click the floating buttons. On the Quest, point a controller at a button and pull the trigger.

## Notes

- WebXR only starts on a secure (HTTPS) page, which is why the rooms are served from GitHub Pages rather than a local server.
- Comfort: walking in VR blinks to the new spot instead of gliding, which avoids motion sickness.
- The budget room can be balanced at $3,200 and $4,500 a month (each need is chosen once; cheaper options like a roommate or a used car make it possible). At $2,400 it can't: even the cheapest needs are 66% of take-home pay, over the 50% the rule allows - a real lesson about who 50/30/20 works for.

## Run locally

Any static server works, for example:

```bash
python -m http.server 8000
```

Then open http://localhost:8000. Desktop mode works over plain HTTP; VR mode on a headset needs the HTTPS address above.
