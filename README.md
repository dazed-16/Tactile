# Tactile

Tactile is a custom split mechanical keyboard for programming, live coding and CAD, with a thumb touchpad for pointer control.

## Why make it?

The aim is a keyboard that feels personal and comfortable during long desk sessions. A split layout lets each hand rest at its own angle, while thumb controls reduce trips between the keyboard and mouse. Tactile switches give clear feedback, and printed keycaps and a case leave room for customization.

## How it works

A wireless controller connects to the computer over Bluetooth. A ribbon cable joins the two halves, and the controller scans the key matrix. The right thumb controls the touchpad; left-thumb keys handle mouse clicks. Layers provide the remaining keyboard functions.

## Challenges so far

Fitting the thumb keys and touchpad into a useful layout has meant balancing comfort with space for the electronics. Another challenge has been choosing a controller and expanding its pins to handle both the keyboard and pointing device. Matching component footprints and keeping the parts affordable still need attention.

The project is in the design stage. The boards and schematics are present; firmware and the physical build are still ahead.

## Design pictures

![Split keyboard layout](docs/images/split-layout.png)

![Left PCB layout](docs/images/left-pcb-layout.png)

![Left PCB 3D preview](docs/images/left-pcb-3d.png)

![Right PCB layout](docs/images/right-pcb-layout.png)

![Right schematic](docs/images/right-schematic.png)

## Files

Open the left and right projects under `Tactile/PCB/` in KiCad. Custom libraries are in `Tactile/Libraries/`, and printable geometry is in `Tactile/Model/`. The purchase list is also available as [BOM.csv](BOM.csv).

Gerbers and drill files are in the [left fabrication folder](Tactile/PCB/Left%20side/fabrication/) and [right fabrication folder](Tactile/PCB/Right%20side/fabrication/), with a ZIP package for each half. These are design exports; fabrication checks are still pending.

## Purchase BOM

All amounts are USD. Unit price is per listed purchase unit; line total already includes quantity. Component prices are earlier estimates except the diode price, rechecked against DigiKey. Unquoted charges are TBD, not zero.

| Component or charge | Buy quantity | Unit USD | Line total USD | Source |
| --- | --- | --- | --- | --- |
| BLE controller | 1 | 9.90 | 9.90 | [Part](https://www.seeedstudio.com/Seeed-XIAO-BLE-nRF52840-p-5201.html) |
| Tactile switches | 2 packs | 9.99 | 19.98 | [Part](https://en.akkogear.com/product/creamy-purple-u1-switch/) |
| Touchpad | 1 | 9.63 | 9.63 | [Part](https://www.mouser.com/en/ProductDetail/Cirque/TM040040-2024-302?qs=wd5RIQLrsJgMzmw571gvDw%3D%3D) |
| Matrix diodes | 100 | 0.0665 | 6.65 | [Part](https://www.digikey.com/en/products/detail/diodes-incorporated/1N4148W-7-F/815280) |
| Shift registers | 2 | 0.30 | 0.60 | [Part](https://www.digikey.com/en/products/detail/nexperia-usa-inc/74HC595D-118/763394) |
| Capacitors | 10 | 0.098 | 0.98 | [Part](https://www.digikey.com/en/products/detail/yageo/CC0805KRX7R9BB104/302874) |
| Touchpad connector | 1 | 2.00 | 2.00 | [Part](https://www.digikey.com/en/products/detail/hirose-electric-co-ltd/FH12-12S-0-5SH-55/1110316) |
| Touchpad cable | 1 | TBD | TBD | [Part](https://www.digikey.com/en/products/detail/assmann-wsw-components/AFFC-050-12-051-11/6570261) |
| Ribbon cable | 2 feet | 1.79 | 3.58 | [Part](https://www.digikey.com/en/products/detail/assmann-wsw-components/AWG28-14-F-300/655738) |
| IDC sockets | 2 | 0.60 | 1.20 | [Part](https://www.digikey.com/en/products/detail/assmann-wsw-components/AWP-14-8240-T/5244612) |
| IDC strain reliefs | 2 | 0.10 | 0.20 | [Part](https://www.digikey.com/en/products/base-product/assmann-wsw-components/123/AWZ/567962) |
| IDC headers | 2 | 0.63 | 1.26 | [Part](https://www.digikey.com/en/products/detail/assmann-wsw-components/AWHW-14G-0202-T/5224931) |
| Power switch | 1 | 0.72 | 0.72 | [Part](https://www.digikey.com/en/products/detail/e-switch/EG1218/101726) |
| Battery | 1 | 9.95 | 9.95 | [Part](https://www.digikey.com/en/products/detail/adafruit-industries-llc/258/5054544) |
| USB cable | 1 | 4.95 | 4.95 | [Part](https://www.adafruit.com/product/4474) |
| Battery protection IC | 1 | TBD | TBD | [Part](https://www.ti.com/product/BQ2970) |
| Dual MOSFET | 1 | TBD | TBD | [Part](https://www.ti.com/product/CSD83325L) |
| 330 ohm resistor | 1 | TBD | TBD | To select |
| 2.2 kOhm resistor | 1 | TBD | TBD | To select |
| Battery connector | 1 | TBD | TBD | [Part](https://www.jst-mfg.com/product/index.php?series=ACH) |
| DigiKey shipping | 1 | 30.00 | 30.00 | [Part](https://www.digikey.com.mx/en) |
| Seeed shipping | 1 | TBD | TBD | [Part](https://support.seeedstudio.com/knowledgebase/topics/56172-shipping) |
| Akko shipping | 1 | TBD | TBD | [Part](https://en.akkogear.com/faq/how-many-days-will-the-delivery-take-if-i-order-today/) |
| Mouser shipping | 1 | TBD | TBD | [Part](https://www.mouser.mx/es/saleterms/) |
| Adafruit shipping | 1 | TBD | TBD | [Part](https://www.adafruit.com/shippinginfo) |
| Tax and import charges | 1 | TBD | TBD | [Part](https://wwwmatnp.sat.gob.mx/articulo/43379/articulo-27) |

DigiKey cut-tape diodes: **100 × $0.06650 = $6.65**, with no Digi-Reel service selected.

Shipping uses the existing supplier list. DigiKey's $30 is its published Mexico rate for orders below $100, subject to checkout and any special-item surcharge. Other shipping needs checkout quotes. Tax/import charges need the final invoice, origin and carrier assessment; a blanket percentage has not been invented.

Known-price components: **$71.60**. With the DigiKey shipping estimate: **$101.60**, plus all TBD parts, shipping and tax. This is a partial amount, not a complete order total.
