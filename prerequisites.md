# Začínáme s OpenCore

Než se vrhneme po hlavě do tvorby systému založeného na OpenCore, musíme si projít několik věcí.

## Předpoklady

1. <span style="color:red">_**[CRUCIAL]**_</span> Čas a trpělivost.
   * Nezačínejte na tom pracovat, pokud máte termíny odevzdání nebo důležitou práci. Hackintoshe nejsou něco, na co byste se jako pracovní stroj měli spoléhat.
2. <span style="color:red">_**[CRUCIAL]**_</span> **ZJISTĚTE SVŮJ HARDWARE**
   * Název vašeho procesoru a jeho generace
   * Vaše grafické karty
   * Vaše úložná zařízení (HDD/SSD, konfigurace NVMe/AHCI/RAID/IDE)
   * Model vašeho notebooku/stolního počítače, pokud je od výrobce OEM
   * Váš **ethernetový čipset**
   * Váš WLAN/Bluetooth čipset 
3. <span style="color:red">_**[KLÍČOVÉ]**_</span> **ZÁKLADNÍ ZNALOSTI PŘÍKAZOVÝCH ŘÁDKŮ A JAK POUŽÍVAT TERMINÁL/PŘÍKAZOVÝ ŘÁDEK**
   * To není jen [KLÍČOVÉ], to je základ celé této příručky. Nemůžeme vám pomoci, pokud nevíte, jak udělat `cd` do adresáře nebo jak smazat soubor.
4. <span style="color:red">_**[KLÍČOVÉ]**_</span> Stroj, který je kompatibilní, jak je vidět v části _**Kompatibilita**_.
   * [Stránka Hardwarová omezení](macos-limits.md)
5. <span style="color:red">_**[KLÍČOVÉ]**_</span> Minimálně:
   * USB disk s kapacitou 16GB, pokud budete k vytvoření USB používat macOS
   * USB disk s kapacitou 4GB, pokud budete pro vytváření USB používat Windows nebo Linux
6. <span style="color:red">_**[KLÍČOVÉ]**_</span> **Ethernetové připojení** (žádné Wi-Fi převodníky, ethernetový USB adaptér může fungovat v závislosti na podpoře macOS) a musíte znát model své LAN karty
   * Musíte mít buď fyzický ethernetový port, nebo kompatibilní ethernetový převodník/adaptér macOS. V případě, že máte [kompatibilní Wi-Fi kartu](https://dortania.github.io/Wireless-Buyers-Guide/), můžete ji také použít.
     * Mějte na paměti, že většina WiFi karet není podporována systémem macOS
   * Pro lidi, kteří nemohou používat ethernet, ale mají telefon se systémem Android, můžete svůj Android telefon připojit k síti Wi-Fi a poté jej přidělit pomocí USB s [HoRNDIS](https://joshuawise.com/horndis#available_versions).
7. <span style="color:red">_**[KLÍČOVÉ]**_</span> **Správná instalace OS:**
   * Musíte mít:
     * macOS (trochu novější by byl lepší)
     * Windows (Windows 10, 1703 nebo novější)
     * Linux (Čistý a správně fungující s Pythonem 2.7 nebo novějším)
   * Pro uživatele systému Windows nebo Linuxu - **15 GB** volného místa na disku, na kterém pracujete. V systému Windows musí mít váš disk s operačním systémem (C:) alespoň **15 GB** volného místa.
   * Pro uživatele macOS **30 GB** volného místa na systémovém disku.
   * Většina nástrojů používaných v této příručce bude také vyžadovat [nainstalovaný Python](https://www.python.org/downloads/)
8. <span style="color:red">_**[KLÍČOVÉ]**_</span> **Nainstalovaný nejnovější BIOS**
   * Ve většině případů nejlepší podporu pro macOS poskytne aktualizace systému BIOS
   * Výjimkou jsou základní desky AMD řady MSI 500, více na [Podpora základních desek](macos-limits.md#motherboard-support)
