# Figma Design

Read directly from the Figma file by Learning Copilot. Every fact here comes
from the design itself rather than from looking at a picture of it, so layer
names, spacing and design-token references are exact.

## Artboards

| Artboard | Width | Height |
|---|---|---|
| Desktop  | 1920px | 7221px |
| iPad Pro 12.9" - 1 | 846px | 9065px |
| iPhone 17 - 1 | 713px | 8887px |

## Tokens by mode — Primitives

These vary across **Desktop** / **Tablet** / **Mobile**. This is how the
designer said the design should change; prefer these over inventing values.

| Token | Desktop | Tablet | Mobile |
|---|---|---|---|
| Sunrise Yellow/100 | #F8EFD1 | #F8EFD1 | #F8EFD1 |
| Sunrise Pink/100 | #FACFEA | #FACFEA | #FACFEA |
| Sunrise Pink/400 | #EB41AB | #EB41AB | #EB41AB |
| Sunrise Pink/700 | #8A0A5A | #8A0A5A | #8A0A5A |
| Sunset Purple/400 | #776AC1 | #776AC1 | #776AC1 |
| Sunset Purple/800 | #221C47 | #221C47 | #221C47 |
| Sunset Blue/800 | #141836 | #141836 | #141836 |
| Sunset Blue/900 | #0A0C1B | #0A0C1B | #0A0C1B |
| Banner & Footer Font Size | 96px | 68px | 48px |
| Corner Radius | 32px | 24px | 16px |
| Card Font Size | 24px | 16px | 12px |
| Side of Image Font Size | 36px | 24px | 16px |
| Fancy font | Italianno | Italianno | Italianno |
| Sans font | Instrument Sans | Instrument Sans | Instrument Sans |

## Tokens by mode — Semantics

These vary across **Light** / **Dark**. This is how the
designer said the design should change; prefer these over inventing values.

| Token | Light | Dark |
|---|---|---|
| Background | Sunrise Pink/400 | Sunset Blue/800 |
| On Background | Sunset Purple/800 | Sunrise Yellow/100 |
| H1 | Sunrise Pink/100 | Sunset Blue/800 |
| On Page Background | Sunrise Yellow/100 | Sunset Blue/900 |
| Page Background | Sunrise Pink/700 | Sunset Purple/400 |
| Light Visible | true | false |
| Dark Visible | false | true |

## Tokens by mode — Type & Sizing

These vary across **Desktop** / **Tablet** / **Mobile**. This is how the
designer said the design should change; prefer these over inventing values.

| Token | Desktop | Tablet | Mobile |
|---|---|---|---|
| Banner & Footer Font Size | 96px | 68px | 48px |
| Corner Radius | 32px | 24px | 8px |
| Card Font Size | 24px | 24px | 16px |
| Side of Image Font Size | 36px | 24px | 16px |
| Fancy font | Italianno | Italianno | Italianno |
| Sans font | Instrument Sans | Instrument Sans | Instrument Sans |

## Page structure

Indentation is nesting. `tokens:` names the design variable bound to that
property — generated CSS should reference that variable rather than repeat a
literal value.

### Desktop 

_Figma page: Desktop/Tablet/Mobile_

- FRAME "Banner" · horizontal stack, gap 10, padding 11 4, justify center, align center · tokens: fills=On Background
  - FRAME "TextContainer" · horizontal stack, padding 18 0, justify center, align center
    - TEXT "A.Vand his" · tokens: fills=H1, fontSize=Banner & Footer Font Size, textRangeFills=H1
    - TEXT "unSmart City" · tokens: fills=H1, fontSize=Banner & Footer Font Size
- FRAME "Image1 Section" · horizontal stack, gap 10, padding 22 98, justify center, align center · tokens: fills=Page Background
  - FRAME "Mega Frame " · horizontal stack, gap 60, padding 25 0, justify center, align center
    - FRAME "Image1Container" · horizontal stack, gap 10, padding 0 15, justify center, align center · tokens: topLeftRadius=Corner Radius, topRightRadius=Corner Radius, bottomLeftRadius=Corner Radius, bottomRightRadius=Corner Radius
      - RECTANGLE "SleepyVucicLight 1" · 942×514 · tokens: visible=Light Visible
    - FRAME "TextContainer" · horizontal stack, gap 10, align center
      - TEXT "Once upon a time, A.V was tossingand turning all night long" · tokens: fills=On Page Background, fontSize=Side of Image Font Size
        text: "Once upon a time, A.V was tossing and turning all night long. He just couldn’t get to sleep! Until finally, his heavy ey"
- FRAME "Image 2 Section" · horizontal stack, gap 10, padding 22 98 38 98, justify center, align center · tokens: fills=Background
  - FRAME "Mega Frame 2" · horizontal stack, gap 60, justify center, align center
    - FRAME "TextContainer" · horizontal stack, gap 10, justify space-between, align center
      - TEXT · tokens: fills=On Background, fontSize=Side of Image Font Size
        text: "He found himself in a familiar street. But he had a pram! ”A pram?” he thought. “I don’t know where this came from, but "
    - FRAME "Image2Container" · horizontal stack, gap 10, padding 33 28, align center · tokens: topLeftRadius=Corner Radius, topRightRadius=Corner Radius, bottomLeftRadius=Corner Radius, bottomRightRadius=Corner Radius
      - RECTANGLE "PramLight 2" · 770×420 · tokens: visible=Light Visible, topLeftRadius=Corner Radius, topRightRadius=Corner Radius, bottomLeftRadius=Corner Radius, bottomRightRadius=Corner Radius
- FRAME "Image 3-5 Section" · horizontal stack, gap 10, padding 12 142, justify center, align center · tokens: fills=Page Background
  - FRAME "Image Container" · horizontal stack, gap 94, padding 47 0, justify center, align center
    - FRAME "Image3Container" · tokens: topLeftRadius=Corner Radius, topRightRadius=Corner Radius, bottomLeftRadius=Corner Radius, bottomRightRadius=Corner Radius, fills=Background
      - FRAME "TextContainer" · horizontal stack, gap 10, padding 33 0, justify center, align center
        - TEXT · tokens: fills=On Background, fontSize=Card Font Size
          text: "He tried taking the pram to the nearest hospital, but there was no ramp. ”How ever will I get in?” Thought A.V. But he j"
      - RECTANGLE "HospitalLight 2" · 508×677 · tokens: visible=Light Visible
    - FRAME "Image4Container" · tokens: topLeftRadius=Corner Radius, topRightRadius=Corner Radius, bottomLeftRadius=Corner Radius, bottomRightRadius=Corner Radius, fills=Background
      - FRAME "TextContainer"
        - TEXT · tokens: fills=On Background, fontSize=Card Font Size
          text: "He continued on and came by a crosswalk. He pressed the button but the light never went green! “I can hear the crossing "
      - RECTANGLE "NoCrossingSoundLight 1" · 590×788 · tokens: visible=Light Visible
    - FRAME "Image5Container" · tokens: topLeftRadius=Corner Radius, topRightRadius=Corner Radius, bottomLeftRadius=Corner Radius, bottomRightRadius=Corner Radius, fills=Background
      - FRAME "TextContainer"
        - TEXT · tokens: fills=On Background, fontSize=Card Font Size
          text: "He ran across the road and found a store, but it was empty. “Guess I’ll just keep going!” He turned around and almost sl"
      - RECTANGLE "StairsToHellLight 2" · 563×750 · tokens: visible=Light Visible
- FRAME "Image 6 Section" · horizontal stack, gap 10, padding 68 76, justify center, align center · tokens: fills=Background
  - FRAME "Mega Frame 3" · horizontal stack, gap 72, padding 20 21, justify center, align center
    - FRAME "Image6Container" · tokens: topLeftRadius=Corner Radius, topRightRadius=Corner Radius, bottomLeftRadius=Corner Radius, bottomRightRadius=Corner Radius
      - RECTANGLE "CarLight 1" · 820×615 · tokens: visible=Light Visible
    - FRAME "TextContainer" · horizontal stack, justify center, align center
      - TEXT · tokens: fills=On Background, fontSize=Side of Image Font Size
        text: "He managed to get down without a single scratch! “To the bus stop!” He thought, but was yet again faced with a challenge"
- FRAME "Image 7-8 Section" · horizontal stack, gap 10, padding 12 142, justify center, align center · tokens: fills=Page Background
  - FRAME "Mega Frame 4" · horizontal stack, gap 10, padding 45 0, justify center, align center
    - FRAME "Mega Frame 5" · horizontal stack, gap 55, justify center, align center
      - FRAME "Image and text container 1"
        - FRAME "TextContainer"
          - TEXT "“Ah yes, the bus stop! I made sure to make this one smart! " · tokens: fills=On Page Background, fontSize=Card Font Size
            text: "“Ah yes, the bus stop! I made sure to make this one smart! I placed a digital timetable at every one!But wait...Why can’"
        - FRAME "Image7Container" · tokens: topLeftRadius=Corner Radius, topRightRadius=Corner Radius, bottomLeftRadius=Corner Radius, bottomRightRadius=Corner Radius
          - RECTANGLE "UnSmartBusLight 1" · 562×749 · tokens: visible=Light Visible
      - FRAME "Image and text container 2"
        - FRAME "TextContainer"
          - TEXT · tokens: fills=On Page Background, fontSize=Card Font Size
            text: "He stared out the window as he passed through his city. Smiling from ear to ear. But then he was abruptly jolted in his "
        - FRAME "Image8Container" · tokens: topLeftRadius=Corner Radius, topRightRadius=Corner Radius, bottomLeftRadius=Corner Radius, bottomRightRadius=Corner Radius
          - RECTANGLE "NoPotHoleLight 1" · 638×850 · tokens: visible=Light Visible
- FRAME "Image 9 Section" · horizontal stack, gap 10, padding 38 196 38 188, justify center, align center · tokens: fills=Background
  - FRAME "Mega Frame 6" · horizontal stack, gap 64, padding 0 40, justify center, align center
    - FRAME "TextContainer" · vertical stack, gap 10, padding 16 6, justify center, align center
      - TEXT · tokens: fills=On Background, fontSize=Side of Image Font Size
        text: "The more challenges he faced, the more he began to blame the incompetence on others. “I gave them everything they need! "
    - FRAME "Image9Container" · vertical stack, gap 10, justify center, align center · tokens: topLeftRadius=Corner Radius, topRightRadius=Corner Radius, bottomLeftRadius=Corner Radius, bottomRightRadius=Corner Radius
      - RECTANGLE "NoRampLight 1" · 531×708 · tokens: visible=Light Visible
- FRAME "Image 10 Section" · horizontal stack, gap 10, padding 14 124 14 168, justify center, align center · tokens: fills=Page Background
  - FRAME "Mega Frame 7" · horizontal stack, gap 39, padding 35 0, justify center, align center
    - FRAME "Image10Container" · tokens: topLeftRadius=Corner Radius, topRightRadius=Corner Radius, bottomLeftRadius=Corner Radius, bottomRightRadius=Corner Radius
      - RECTANGLE "MoneyLight 1" · 982×535 · tokens: visible=Light Visible
    - FRAME "TextContainer"
      - TEXT · tokens: fills=On Page Background, fontSize=Side of Image Font Size
        text: "Amidst all the chaos of thoughts and woes, it suddenly dawned on him that he never checked on the baby. He leaned over a"
- FRAME "Text Only Section" · horizontal stack, gap 10, padding 8 116, justify center, align center · tokens: fills=Background
  - FRAME "Mega Frame 8" · horizontal stack, gap 10, padding 24 35, justify center, align center
    - FRAME "TextOnlyContainer" · horizontal stack, gap 10, padding 25 28, justify center, align center · tokens: topLeftRadius=Corner Radius, topRightRadius=Corner Radius, bottomLeftRadius=Corner Radius, bottomRightRadius=Corner Radius, fills=Page Background
      - FRAME "TextContainer" · horizontal stack, gap 10, justify center, align center
        - TEXT · tokens: fills=On Page Background, fontSize=Side of Image Font Size
          text: "Just as he entered the building, his alarm began to ring. A.V awoke in a pool of sweat, breathing heavily as if he had b"
- FRAME "Image 11 Section" · horizontal stack, gap 10, padding 14 316, justify center, align center · tokens: fills=Page Background
  - FRAME "Mega Frame 9" · vertical stack, gap 20, justify center, align center
    - FRAME "Image11Container" · vertical stack, justify center, align center · tokens: topLeftRadius=Corner Radius, topRightRadius=Corner Radius, bottomLeftRadius=Corner Radius, bottomRightRadius=Corner Radius
      - RECTANGLE "MoneyBedLight 2" · 1288×703 · tokens: visible=Light Visible
    - FRAME "TextContainer" · vertical stack, gap 10, padding 6 14, justify center, align center
      - TEXT · tokens: fills=On Page Background, fontSize=Side of Image Font Size
        text: "Luckily for him, he never had a change of heart at all! The taxpayer’s money remains safe with him for another day, and "
- FRAME "Footer Section" · horizontal stack, gap 10, padding 23 80 23 116, justify center, align center · tokens: fills=On Background
  - FRAME "Mega Frame 10" · horizontal stack, padding 0 39 0 49, justify center, align center
    - TEXT "This wouldn’t have been possible" · tokens: fills=H1, fontSize=Banner & Footer Font Size
    - TEXT "without you, A.V!" · tokens: fills=H1, fontSize=Banner & Footer Font Size, textRangeFills=H1

## Tokens used in this page

10 across 77 layers:

`Background`, `Banner & Footer Font Size`, `Card Font Size`, `Corner Radius`, `H1`, `Light Visible`, `On Background`, `On Page Background`, `Page Background`, `Side of Image Font Size`
