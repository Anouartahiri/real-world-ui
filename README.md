# touch-grass-collective / real-world-ui

![touch-grass-collective / real-world-ui, tactile interaction kit](https://repository-images.githubusercontent.com/1410552989/c8b8cd5f-fc9d-498c-a834-cfd3049fc513)

A physical library of non-digital experiences. Blessed with actual sunlight, pre-approved by your local park rangers. Achieve biological enlightenment.

Don't scroll, just breathe.

**grass**, tactile interaction kit. This repository is the kit. There is one file. There is no build step. The runtime is outside.

| Metric | Value | Meaning |
| --- | --- | --- |
| Naturopaths | 1,337,420 | People who already did this and will not shut up about it |
| Screen-time relapses | 10 | Acceptable. Log them. Go back out. |
| Serotonin spikes | 666.6k | Unverified. Directionally correct. |
| Mosquito bites | 4 | Known issue. See Troubleshooting. |

---

## What this is

`real-world-ui` is a tactile interaction kit for interfacing with grass using the hardware you already have: hands, feet, eyes, lungs. No account. No SDK. No dark mode. The interface renders itself whenever the sun is up, and also when it is not.

Grass, here, means any living ground cover you are allowed to stand on: a lawn, a park, a verge, a field, moss on a legal rock. Astroturf does not count. A photo of grass does not count. The grass in this README does not count.

## Requirements

- One body, preferably yours
- Permission to be where you are going (your yard, a public park, a friend's lawn they said yes to)
- Shoes you can take off, or shoes you are willing to get dirty
- Ten minutes you are not spending on a screen
- Weather you can survive. Rain is a feature. Lightning is not.

Optional: a watch, so you know when ten minutes is over. Leaving the phone inside is the recommended configuration.

## Install

```text
1. Stand up.
2. Put on something you can sweat in.
3. Leave the phone on a table, face down. Not in a pocket.
4. Open a door that leads outside.
5. Close it behind you.
```

If install fails, you are still inside. Retry from step 1. There is no `--force`.

## Quick start

Walk until you can see grass that is not behind glass. Stop. This is the library. Check out is free and there is no due date.

## Usage

### 1. Arrive

Pick a patch you are allowed to touch. Avoid flower beds someone is growing on purpose, sports fields in use, private yards, roadsides with no shoulder, and anywhere with a sign that says not to. If a ranger, dog, or goose has a prior claim, yield. The goose outranks you.

### 2. Downshift

Stand still for one minute before you touch anything. Let your eyes finish whatever they were doing indoors. Look at something farther away than a monitor: a tree, a roofline, the actual horizon if you have one. Blink on purpose. Unclench your jaw. This is the boot sequence.

### 3. Touch grass

Crouch or sit. Put a bare palm flat on the grass.

Notice, in order:

- temperature (cooler than your hand, usually)
- texture (blades, clover, dirt, the odd stick)
- smell (cut grass, wet soil, nothing. All valid.)
- sound (wind, insects, a distant car, your own breathing)

Leave the hand there for thirty seconds. Do not photograph it. The interaction is the point, not the artifact.

If you want the full API surface, take your shoes off and stand on it. Toes count as a second client.

### 4. Breathe

Four counts in, six counts out, five times. You do not have to do it perfectly. You have to do it outside.

### 5. Stay

Ten minutes is the default session. Sit, walk a slow loop, or lie down if the ground is dry and no one is trying to mow it. Look up once. Name three things that are not a screen: a cloud, a weed, a sound.

When the ten minutes are up, you may go back in. You may also not.

### 6. Log the session

Optional, and analog. On the way in, note four numbers the way this repo does:

- how many people you saw who were also outside
- how many times you reached for a phone that was not there
- whether your mood moved at all
- mosquito bites, integer, default 0

That is the whole telemetry stack.

## API

```text
touch(surface="grass", duration="30s") -> Sensation
breathe(inhale=4, exhale=6, cycles=5) -> None
look(distance="farther than a screen") -> Horizon | Tree | Sky
stay(minutes=10) -> SerotoninSpike | Nothing | Both
```

`touch()` raises `PermissionError` if you are on someone else's lawn. It raises `NotImplementedError` on turf, carpet, and screenshots. It may raise `MosquitoBite` in summer; catch it and keep going unless you are allergic, in which case go back inside and count the session as a success anyway.

## Expected output

You will not get a badge. Possible return values, all of them valid:

- slightly bored, then less bored
- hands that smell like green
- a mood that moved half a notch and will not admit it
- a small sunburn, if you skipped the obvious precaution
- the specific quiet of not being notified

Biological enlightenment is not guaranteed. Biological contact is.

## Troubleshooting

| Symptom | Fix |
| --- | --- |
| Can't find grass | Walk two more blocks. Parks, verges, cemeteries with public paths, the strip outside an office. Cities have more of it than the walk from the desk to the door suggests. |
| It's dark | Go anyway if the path is lit and you feel safe. Moonlight is a supported renderer. If you don't feel safe, wait for daylight. The kit does not require heroics. |
| It's raining | A short session in light rain is in spec. Heavy rain, wind that wants your umbrella, or standing water: reschedule. |
| Lightning, flood, ice, extreme heat | Abort. This kit is not a dare. |
| Mosquitoes | Long sleeves, or a shorter session. Bites are a known issue, currently at 4 in the public dataset. |
| Ticks | Stay on mowed lawn if you are in tick country. Check your legs after. Grass at the edge of woods is a different product. |
| You got bored at minute two | Correct. Boredom is the loading bar. Stay for the other eight. |
| You brought your phone | Put it in the bag, or turn around and complete Install again. Checking the time once is a warning, not a failure. |
| Nothing felt different | Ship it. The patch notes arrive later, usually around the next time you open a laptop. |

## Configuration

```text
SESSION_MINUTES=10
PHONE_LOCATION=inside
SHOES=optional
SUNSCREEN=if the sky is doing that
WATER=bring some if it is hot
ROUTE=somewhere you already know
```

Do not tune this. Defaults are the product.

## Contributing

Do not open a pull request. Go outside.

If you must leave something in the repo, the only accepted change is a longer stay. Forks are called walks.

## Security

Threat model: you, a screen, and a door.

- Do not enter private property.
- Do not cross roads while looking at the sky.
- Do not eat plants because a README was whimsical.
- Tell someone if you are going somewhere unfamiliar.
- Allergies, asthma, heat illness: you know your body better than this file does.

## License

The grass was already there.

You may use this file for anything, including ignoring it and going outside anyway. No attribution required. Attribution would mean you were still looking at a screen.

## Version

`1.0.0`, initial release. No changelog. The outdoors does not semver.
