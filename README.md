 # 📗 Algerudi Pebblewhisk’s Grand Guide to GnoScript™ and GnoClassical™

Whether you're a humble boiler fixer or a blueprint architect of wild whirlygigs, this guide will walk you through **both the basic scripting style** of GnoScript and the **object-oriented wizardry** of GnoClassical™.

Let’s begin—mind the sparks!

---

## 🧰 Core Concepts (For All Good Tinkerers)

| Concept Type     | Scripting Mode         | OOP Mode (GnoClassical) |
| ---------------- | ---------------------- | ----------------------- |
| Variable         | `set`                  | `set cog`               |
| Function         | `thing`                | `tool`                  |
| Conditional      | `maybe` / 'unless' / `otherwise`  | Same                    |
| Loop             | `again`                | Same                    |
| Boolean Values   | `spinning` / `stopped` | Same                    |
| Object           | —                      | `widget`                |
| Class Definition | —                      | `blueprint`             |
| Constructor      | —                      | `when_built`            |

---

## 📝 GnoScript (Basic Scripting)

### 🔹 Variables & Sayings

```gno
set power to 10
say "Power level is " + power
```

### 🔹 Conditionals

```gno
maybe power > 5
  say "That's a spicy spark!"
unless power > 10
  say "That's a lot of power!"
otherwise
  say "Needs more juice."
```

### 🔹 Loops

```gno
again 3 times
  say "Whirrr..."
```

### 🔹 Things (Simple Functions)

```gno
thing shout_twice with msg
  say msg
  say msg

tell = shout_twice with "Incoming!"
```

---

## 🧱 GnoClassical™ (Object-Oriented Blueprinting)

### 🔹 Defining a Blueprint

```gno
blueprint Kettle
  set cog heat to 0

  tool boil
    say "Boiling..."
    set me.heat to 100

  tool check
    maybe me.heat == 100
      say "Ready for tea!"
    otherwise
      say "Still warming..."

  when_built
    say "Kettle constructed."
```

### 🔹 Creating and Using Widgets

```gno
set widget my_kettle to new Kettle
my_kettle.boil()
my_kettle.check()
```

### 🔹 Tool Parameters

```gno
tool refuel with amount
  set me.fuel to me.fuel + amount
```

### 🔹 Inheritance (Optional Madness)

```gno
blueprint Teapot implements Kettle
  tool whistle
    say "Fweeeeeeee!"
```

### 🔹 Private Cogs

```gno
set hidden_cog password to "tealover3000"
```

---

## 🧩 Full Example: Rocket Logic in Both Styles

### Basic Style

```gno
set charge to 0
again 4 times
  set charge to charge + 25

maybe charge == 100
  say "Launch ready!"
otherwise
  say "Try again later."
```

### OOP Style

```gno
blueprint Rocket
  set cog fuel to 0

  tool refuel with amount
    set me.fuel to me.fuel + amount

  tool launch
    maybe me.fuel >= 100
      say "Launching!"
    otherwise
      say "Not enough fuel."

  when_built
    say "Rocket ready for fueling."

set widget booster to new Rocket
booster.refuel with 50
booster.launch()
```

---

## Final Words

* Use **basic GnoScript** for quick puzzles, scenes, and silly logic.
* Use **GnoClassical™** for larger gadgets, reusable machines, and boss-worthy contraptions.
* Don’t forget: booleans are `spinning` or `stopped`, not `true` or `false`—what do you think this is, elf-code?

Now off with you! Go script, weld, compile, or explode something *with style!*
