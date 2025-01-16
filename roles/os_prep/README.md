# OS_PREP

### 1. `encrypt_disk.yml/encrypt_partition.yml`

#### Файлы: 
`roles/os_prep/tasks/encrypt_disk.yml`
`roles/os_prep/tasks/encrypt_partition.yml`

This tasks is responsible for encrypting a specified disk or partition next to root partition using LUKS.

## Parameters

- `second_disk`: The disk or partition to encrypt (e.g., `/dev/sdb`).

## Usage

1. Define the `second_disk` variable in your inventory or playbook.


---

### 2. `disable_c_state`

#### Файл: `roles/os_prep/tasks/disable_c_state.yml`
```markdown
# Disable C-State

This task disables C-state for all CPUs to improve performance.
```

---

### 3. `cpu_performance.yml`

#### Файл: `roles/os_prep/tasks/cpu_performance.yml`
```markdown
# Set CPU Performance Mode

This task switches the CPU to performance mode.
```

---

### 4. `rename_network.yml`

#### Файл: `roles/os_prep/tasks/rename_network.yml`
```markdown
# Rename Network Interface

This task renames the active network interface to `net0`.
```


---

### 5. `display_cpu_info.yml`

#### Файл: `roles/os_prep/tasks/display_cpu_info.yml`
```markdown
# Display CPU Information

This task displays information about the CPUs, including Hyper-Threading status.
```
