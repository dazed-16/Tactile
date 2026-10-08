# Tactile v1 — bill of materials

**Revision:** 2026-10-07 · **Status:** design-stage purchasing reference, not order-ready.

Tactile is an open-source split keyboard for programming, live coding and Onshape CAD. The v1 baseline uses one nRF52840 BLE controller, a cable-connected passive half, a right-thumb Cirque touchpad, left-thumb mouse-click keys and integrated matrix macro keys. Keycaps and enclosure are planned for home 3D printing.

## Purchased parts

All numeric prices are **USD**, before shipping, tax/customs and currency-conversion fees. Prices are indicative supplier observations recorded during the 2026-10-07 sourcing review, not checkout quotes. Stock and Mexico delivery must be reconfirmed. **TBD means unquoted, not $0.** Quantities are purchase quantities, including spares; the final key count is still open.

| Item | Manufacturer | Part number / model | Purchase qty | Unit price USD | Line total USD | Purchase link | Notes |
| --- | --- | --- | ---: | ---: | ---: | --- | --- |
| BLE controller | Seeed Studio | `102010448` | 1 board | 9.90 | 9.90 | [Supplier](https://www.seeedstudio.com/Seeed-XIAO-BLE-nRF52840-p-5201.html) | Standard XIAO nRF52840; exact board/expanded matrix validation pending. |
| Tactile switches | Akko | `Creamy Purple U1` | 2 packs × 45 | 9.99 / pack | 19.98 | [Supplier](https://en.akkogear.com/product/creamy-purple-u1-switch/) | 90 purchased; final fitted key count TBD. Tactile, not silent. |
| SPI touchpad, 40 mm | Cirque | `TM040040-2024-302` | 1 | 9.63 | 9.63 | [Supplier](https://www.mouser.com/en/ProductDetail/Cirque/TM040040-2024-302?qs=wd5RIQLrsJgMzmw571gvDw%3D%3D) | Exact SPI variant; stock/checkout confirmation required. |
| Matrix diodes, SOD-123 | Diodes Incorporated | `1N4148W-7-F` | 100 | 0.0665 | 6.65 | [Supplier](https://www.digikey.com/en/products/detail/diodes-incorporated/1N4148W-7-F/815280) | One per fitted key; remainder spares. |
| Column shift registers, SOIC-16 | Nexperia | `74HC595D,118` | 2 | 0.30 | 0.60 | [Supplier](https://www.digikey.com/en/products/detail/nexperia-usa-inc/74HC595D-118/763394) | Cut tape; shared-SPI scan implementation unproven. |
| 100 nF X7R 0805 capacitors | YAGEO | `CC0805KRX7R9BB104` | 10 | 0.098 at qty 10 | 0.98 | [Supplier](https://www.digikey.com/en/products/detail/yageo/CC0805KRX7R9BB104/302874) | Initially fit three; remaining spares. |
| 12-pin 0.5 mm FFC connector | Hirose | `FH12-12S-0.5SH(55)` | 1 | 2.00 | 2.00 | [Supplier](https://www.digikey.com/en/products/detail/hirose-electric-co-ltd/FH12-12S-0-5SH-55/1110316) | Bottom contacts; verify cable mating and pin orientation. |
| 12-pin 0.5 mm FFC cable, 50.8 mm | ASSMANN | `AFFC-050-12-051-11` | 1 | TBD | TBD | [Supplier](https://www.digikey.com/en/products/detail/assmann-wsw-components/AFFC-050-12-051-11/6570261) | USD quote missing; same-side contacts candidate, mating not yet approved. |
| 14-way 28 AWG ribbon cable | ASSMANN | `AWG28-14/F/300` | 2 feet | 1.79 / foot | 3.58 | [Supplier](https://www.digikey.com/en/products/detail/assmann-wsw-components/AWG28-14-F-300/655738) | Buy cut length, not a 300-foot spool. |
| 2×7 IDC ribbon sockets | ASSMANN | `AWP 14-8240-T` | 2 | 0.60 | 1.20 | [Supplier](https://www.digikey.com/en/products/detail/assmann-wsw-components/AWP-14-8240-T/5244612) | One per end; crimp and continuity-test. |
| IDC strain reliefs | ASSMANN | `AWZ-14-T` | 2 | 0.10 | 0.20 | [Supplier](https://www.digikey.com/en/products/base-product/assmann-wsw-components/123/AWZ/567962) | Select exact 14-position variant at series link. |
| Keyed 2×7 PCB headers | ASSMANN | `AWHW 14G-0202-T` | 2 | 0.63 | 1.26 | [Supplier](https://www.digikey.com/en/products/detail/assmann-wsw-components/AWHW-14G-0202-T/5224931) | Through-hole; confirm mating drawing/pin 1. |
| SPDT power slide switch | E-Switch | `EG1218` | 1 | 0.72 | 0.72 | [Supplier](https://www.digikey.com/en/products/detail/e-switch/EG1218/101726) | Proposed battery disconnect also disconnects charging when off. |
| Protected 3.7 V 1200 mAh LiPo | Adafruit | `258` | 1 | 9.95 | 9.95 | [Supplier](https://www.digikey.com/en/products/detail/adafruit-industries-llc/258/5054544) | Ground-shipment restriction; Mexico delivery not confirmed. |
| JST-PH battery header, 2 mm | JST | `B2B-PH-K-S(LF)(SN)` | 1 | 0.11 | 0.11 | [Supplier](https://www.mouser.com/en/ProductDetail/JST-Commercial/B2B-PH-K-SLFSN?qs=cdbOS8ANM9AlozzPlOt72g%3D%3D) | USD listing checked 2026-10-07; check actual battery polarity. |
| USB-A to USB-C data cable, ~1 m | Adafruit | `4474` | 1 if not already owned | 4.95 | 4.95 | [Supplier](https://www.adafruit.com/product/4474) | Charging/programming; removable from purchase if owned. |

## Home-made items and unquoted costs

| Item | Part number | Qty | Price USD | Status |
| --- | --- | --- | --- | --- |
| Home-printed MX-compatible keycaps | Custom design, TBD | One per fitted key | TBD filament | No purchased $9.99 set; print one stem-fit sample first. |
| Printed case and plates | Custom design, TBD | One complete split enclosure | TBD filament/hardware | K1 Max available; geometry, feet and fasteners remain open. |
| Keyboard PCBs | Custom KiCad design, TBD | One working left/right pair; order minimum TBD | TBD | JLCPCB quote follows final outline/layers/quantity. |
| Battery hookup leads | Short insulated ribbon offcuts | Two leads if needed | Included in cable allowance | Verify conductor/current suitability and secure leads; XIAO BAT pads need explicit connection. |
| Shipping, taxes/customs and conversion | Not applicable | Per supplier order | TBD | Mexico; approximate postal code 76226, final address not confirmed. |

## Budget

- **Known-price subtotal: $71.71**, including a new USB cable and the newly quoted $0.11 JST battery header.
- **Without purchasing a USB cable: $66.76**.
- Both figures exclude every TBD item above, including the touchpad FFC cable. A full landed total is not yet available.
- Home printing removes the $9.99 retail keycap purchase; it does not make filament free.
- Current grant planning target is $65; $100 is a stretch tier dependent on actual logged work. The present design does not fit a complete $65 budget.

## Design checks before ordering

- Demonstrate expanded matrix scanning and shared SPI operation with the selected controller/firmware.
- Verify FFC thickness, contact side and pin mapping against the exact Cirque module and Hirose connector.
- Confirm a protected battery can actually be delivered to Mexico, its polarity and charger compatibility. Two-week runtime remains a target.
- Finalize layout, thumb fit, cap geometry and case retention; validate footprints against manufacturer drawings.
- Obtain fabrication and consolidated delivery quotes and confirm grant purchasing rules. Distributor stock does not establish JLCPCB assembly eligibility.

The controller/module choice, expansion circuit and cable implementation are proposals awaiting validation. No display, hot-swap sockets, magnetic modularity or second controller/battery are included. PCB/schematic modifications require user approval.

## Work record

Completed on 2026-10-07: consolidated exact part numbers and supplier links; separated unit and purchase prices; accounted for cable mating parts; removed purchased caps from the baseline; verified subtotal arithmetic; identified unresolved compatibility and delivery checks.

**Actual duration of this BOM session: pending the user's time record.** This document provides evidence of work; it does not establish or certify additional grant hours.

Detailed research: [sourcing and component rationale](BOM_V1.md), [schematic preparation](SCHEMATIC_PREP.md).
