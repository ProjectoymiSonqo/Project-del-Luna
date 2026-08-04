# System Architecture

## Design Philosophy

Project del Luna is designed as a digital Goshuin book that combines
embedded systems with cultural experiences.

The goal is not to replace traditional Goshuin books,
but to preserve travel memories through modern technology.

The architecture separates hardware, firmware,
mobile application, and cloud-independent data management,
allowing each component to evolve independently.

---

## High-Level Architecture

            +-----------------------+
            |     Mobile App        |
            | Shrine Database       |
            | User Management       |
            +-----------+-----------+
                        |
                       BLE
                        |
        +---------------v---------------+
        |          STM32U575            |
        |-------------------------------|
        | NFC      E-paper      Flash   |
        +------+-----------+------------+
               |           |
            ST25DV      Waveshare
             NFC         Display

## Software Architecture

Application

↓

NFC Manager

↓

Display Manager

↓

Storage Manager

↓

HAL Drivers