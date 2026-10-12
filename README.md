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

Submission estimate in USD, using the current supplier list and delivery to Mexico. Prices are per listed purchase unit; line totals already include quantity. **Estimated order total: $211.80** ($76.80 components + $95.00 shipping + $40.00 tax/import allowance).

| Component or charge | Buy quantity | Unit USD | Line total USD | Source |
| --- | --- | --- | --- | --- |
| BLE controller | 1 | 9.90 | 9.90 | [Part](https://www.seeedstudio.com/Seeed-XIAO-BLE-nRF52840-p-5201.html) |
| Tactile switches | 2 packs | 9.99 | 19.98 | [Part](https://en.akkogear.com/product/creamy-purple-u1-switch/) |
| Touchpad | 1 | 9.63 | 9.63 | [Part](https://www.mouser.com/en/ProductDetail/Cirque/TM040040-2024-302?qs=wd5RIQLrsJgMzmw571gvDw%3D%3D) |
| Matrix diodes | 100 | 0.0665 | 6.65 | [Part](https://www.digikey.com/en/products/detail/diodes-incorporated/1N4148W-7-F/815280) |
| Shift registers | 2 | 0.30 | 0.60 | [Part](https://www.digikey.com/en/products/detail/nexperia-usa-inc/74HC595D-118/763394) |
| Capacitors | 10 | 0.098 | 0.98 | [Part](https://www.digikey.com/en/products/detail/yageo/CC0805KRX7R9BB104/302874) |
| Touchpad connector | 1 | 2.00 | 2.00 | [Part](https://www.digikey.com/en/products/detail/hirose-electric-co-ltd/FH12-12S-0-5SH-55/1110316) |
| Touchpad cable (estimate) | 1 | 2.00 | 2.00 | [Part](https://www.digikey.com/en/products/detail/assmann-wsw-components/AFFC-050-12-051-11/6570261) |
| Ribbon cable | 2 feet | 1.79 | 3.58 | [Part](https://www.digikey.com/en/products/detail/assmann-wsw-components/AWG28-14-F-300/655738) |
| IDC sockets | 2 | 0.60 | 1.20 | [Part](https://www.digikey.com/en/products/detail/assmann-wsw-components/AWP-14-8240-T/5244612) |
| IDC strain reliefs | 2 | 0.10 | 0.20 | [Part](https://www.digikey.com/en/products/base-product/assmann-wsw-components/123/AWZ/567962) |
| IDC headers | 2 | 0.63 | 1.26 | [Part](https://www.digikey.com/en/products/detail/assmann-wsw-components/AWHW-14G-0202-T/5224931) |
| Power switch | 1 | 0.72 | 0.72 | [Part](https://www.digikey.com/en/products/detail/e-switch/EG1218/101726) |
| Battery | 1 | 9.95 | 9.95 | [Part](https://www.digikey.com/en/products/detail/adafruit-industries-llc/258/5054544) |
| USB cable | 1 | 4.95 | 4.95 | [Part](https://www.adafruit.com/product/4474) |
| Battery protection IC (estimate) | 1 | 1.00 | 1.00 | [Part](https://www.ti.com/product/BQ2970) |
| Dual MOSFET (estimate) | 1 | 1.50 | 1.50 | [Part](https://www.ti.com/product/CSD83325L) |
| 330 ohm resistor (estimate) | 1 | 0.10 | 0.10 | To select |
| 2.2 kOhm resistor (estimate) | 1 | 0.10 | 0.10 | To select |
| Battery connector (estimate) | 1 | 0.50 | 0.50 | [Part](https://www.jst-mfg.com/product/index.php?series=ACH) |
| DigiKey shipping | 1 | 30.00 | 30.00 | [Part](https://www.digikey.com.mx/en) |
| Seeed shipping (estimate) | 1 | 10.00 | 10.00 | [Part](https://support.seeedstudio.com/knowledgebase/topics/56172-shipping) |
| Akko shipping (estimate) | 1 | 15.00 | 15.00 | [Part](https://en.akkogear.com/faq/how-many-days-will-the-delivery-take-if-i-order-today/) |
| Mouser shipping (estimate) | 1 | 20.00 | 20.00 | [Part](https://www.mouser.mx/es/saleterms/) |
| Adafruit shipping (estimate) | 1 | 20.00 | 20.00 | [Part](https://www.adafruit.com/shippinginfo) |
| Tax and import charges (estimate) | 1 | 40.00 | 40.00 | [Part](https://wwwmatnp.sat.gob.mx/articulo/43379/articulo-27) |

The unquoted components and shipping use planning allowances, not supplier quotes. Shipping assumes separate orders from DigiKey, Seeed, Akko, Mouser and Adafruit. DigiKey's $30 follows its published Mexico rate below $100; the remaining shipping allowances are provisional. The $40 tax/import allowance is a budget reserve, not a tax-rate calculation or guaranteed upper bound. Final checkout and carrier charges may differ.

Verified diode price: **100 × $0.06650 = $6.65**, cut tape. Other listed component prices are earlier supplier estimates. No parts order has been placed.
