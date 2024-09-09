---
home: true
heroImage: /dortania-logo-clear.png
heroText: Průvodce instalací OpenCore od Dortania
actionText: Začínáme→
actionLink: prerequisites.md

meta:
- name: popis
  content: Aktuální podporovaná verze je 0.9.1
---

# Co je OpenCore a pro koho je tato příručka určena

OpenCore je to, co nazýváme „bootloader“ – je to komplexní software, který používáme k přípravě našich systémů pro macOS – konkrétně vkládáním nových dat pro macOS, jako jsou SMBIOS, tabulky ACPI a kexty. Jak se tento nástroj liší od jiných, jako je Clover, je to, že byl navržen s ohledem na bezpečnost a kvalitu, což nám umožňuje používat mnoho funkcí zabezpečení, které se nacházejí na skutečných Mac počítačích, jako [Ochrana integrity systému](https://support.apple.com/en-ca/HT204899) a [FileVault](https://support.apple.com/en-ca/HT204837). Podrobnější pohled najdete zde: [Proč OpenCore před Cloverem a dalšími](why-oc.md)

Tato příručka se konkrétně zaměřuje na dvě hlavní věci:

* Instalace macOS na PC na architektuře X86
* Naučí vás, co umožní vašmu Hacku fungovat

Z tohoto důvodu se od vás bude očekávat, že budete číst, učit se a dokonce používat Google. Nejedná se o jednoduché nastavení instalace jedním kliknutím.

Pamatujte, že OpenCore je stále nové a aktuálně ve verzi beta. I když je docela stabilní a pravděpodobně mnohem stabilnější než Clover v podstatě ve všech směrech, stále se často aktualizuje, takže kusy konfigurace se poměrně často mění (tj. nové vtípky nahrazují staré).

A konečně, ti, kteří mají problémy, mohou navštívit [r/Hackintosh subreddit](https://www.reddit.com/r/hackintosh/) a [r/Hackintosh Discord server](https://discord.gg/u8V7N5C) pro další pomoc.
