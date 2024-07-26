# RL-CartPole-A2C-vs-PPO
Dieses Projekt untersucht die Implementierung und Optimierung von Reinforcement Learning (RL) Algorithmen in der CartPole-V1 Umgebung von Gymnasium. Zwei RL-Algorithmen, Advantage Actor-Critic (A2C) und Proximal Policy Optimization (PPO), werden implementiert, verglichen und durch Hyperparameter-Tuning mit Optuna optimiert.

## Inhaltsverzeichnis
- [Einführung](#einführung)
- [Verwendete Packages](#verwendete-packages)
- [Installation](#installation)
- [Verwendung](#verwendung)
- [Visualisierung mit TensorBoard](#visualisierung-mit-tensorboard)
- [Ergebnisse](#ergebnisse)
- [Autor](#autor)
  
## Einführung
Das Ziel dieses Projekts ist es, die Leistung von A2C und PPO in der CartPole-V1 Umgebung zu vergleichen und durch Hyperparameter-Tuning zu optimieren. CartPole-V1 ist eine klassische RL-Umgebung, die verwendet wird, um das Balance-Problem zu demonstrieren.

## Verwendete Packages
- `numpy`
- `gymnasium`
- `stable-baselines3`
- `optuna`
- `torch`
- `tensorboard`

## Installation
Um das Projekt lokal auszuführen, folge diesen Schritten:

1. **Repository klonen:**
   ```bash
   git clone https://github.com/DeanTom/RL-CartPole-A2C-vs-PPO.git
   cd RL-CartPole-A2C-vs-PPO
   
## Verwendung
Um die RL-Entwicklung und die RL-Agenten zu entwickeln und zu trainieren, folge diesen Schritten:

### A2C:

- Ausführen der Datei: `A2C.ipnyb`

### PPO:

- Ausführen der Datei: `PPO.ipynb`

## Visualisierung mit TensorBoard
Um die Trainingsergebnisse mit TensorBoard zu visualisieren, folge diesen Schritten:

1. **In die jeweilige Log-Datei (Logs/A2C_X oder Logs/PPO_X) navigieren:**
   ```bash
   cd Logs/A2C_X oder
   cd Logs/PPO_X
   ```
   - X ist hierbei stets mit dem aktuellen/gewünschten Durchlauf zu ersetzen.

2. **TensorBoard starten:**
   ```bash
   tensorboard --logdir=./

3. **Öffne das TensorBoard-Dashboard:**

    - Gehe zu http://localhost:6006 in deinem Browser, um die Trainingsverläufe und Ergebnisse zu visualisieren.

4. **Anpassen des geloggten Modells (optional):**
    
    - Das Modell (baseline/tuned), welches geloggt werden soll, kann nach Bedarf angepasst werden.
    - Der Parameter ```tensorboard_log = LOG_DIR``` muss dabei lediglich an das gewünschte Modell mitgegeben werden.
    - Standardmäßig ist der Parameter dem Baseline-Modell zugeordnet.
      
## Ergebnisse
Die Ergebnisse des Projekts zeigen, dass der PPO-Algorithmus in der Baseline-Version eine bessere Performance aufweist als der A2C-Algorithmus. Die optimierten Modelle zeigten eine Verbesserung im Vergleich zu den Baseline-Modellen, wobei hier beide Agenten den maximalen Reward der Umgebung von 500 ausreizen.

## Autor
Dean Tomanelli
