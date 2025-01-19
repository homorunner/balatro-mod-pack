# Awesome balatro mod pack

## Install

Run in powershell:

```powershell
cd $env:APPDATA\Balatro

git clone https://github.com/homorunner/balatro-mod-pack.git

if (Test-Path -Path "Mods") {
    Get-ChildItem -Path "Mods" | ForEach-Object {
        Move-Item -Path $_.FullName -Destination "balatro-mod-pack" -ErrorAction Stop
    }
    Remove-Item -Path "Mods" -Recurse -Force -ErrorAction Stop
}

Rename-Item -Path "balatro-mod-pack" -NewName "Mods" -ErrorAction Stop
```

## Mods

### Aurinko

Author: jenwalter666

Github link: https://github.com/jenwalter666/JensBalatroCollection

Planet card can have editions.

### Betmma Voucher Pack

Author: Betmma, nicholassam6425

Github link: https://github.com/betmma/my_balatro_mods

Adds 3 Voucher Packs.

### Cryptid

Author: MathIsFun_, Cryptid and Balatro Discords

Github link: https://github.com/MathIsFun0/Cryptid

A lot of cool new jokers, consumables, blinds and so on.

### Galdur

Author: Eremel

Github link: https://github.com/Eremel/Galdur

Improved startup screen.

### MoreFluff

Author: notmario

Github link: https://github.com/notmario/MoreFluff

Add a new consumable: Color card. Also adds some cool jokers.

### Talisman

Author: MathIsFun_, Mathguy24, jenwalter666, cg-223

Github link: https://github.com/MathIsFun0/Talisman

Increases the score cap, making it hard to reach nan/inf.