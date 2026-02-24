# Pertemuan 02 – Git Advanced Branching Strategies

## Branching Strategies

Pada praktikum ini dipelajari beberapa strategi branching:

- GitFlow
- GitHub Flow
- Trunk-Based Development
- GitLab Flow

GitFlow menggunakan branch utama:
- main (production)
- develop (development)
- feature/*
- release/*
- hotfix/*

## Implementasi GitFlow

Langkah yang dilakukan:

1. Membuat repository dan initial commit
2. Membuat branch develop
3. Membuat feature branch
4. Merge feature ke develop
5. Membuat release branch
6. Merge release ke main
7. Merge kembali ke develop
8. Menambahkan tag v1.0

## Merge Conflict

Conflict dibuat dengan mengubah file login.txt
pada branch develop dan feature-conflict3
dengan isi yang berbeda.

Saat dilakukan merge, Git menampilkan:

CONFLICT (content): Merge conflict in login.txt

Conflict diselesaikan secara manual dengan:
1. Mengedit file
2. Menghapus tanda <<<<<<< ======= >>>>>>>
3. Menyimpan hasil gabungan
4. Melakukan git add dan git commit

## Kesimpulan

GitFlow membantu mengelola branch secara terstruktur.
Merge conflict terjadi ketika dua branch
mengubah bagian file yang sama.
Conflict dapat diselesaikan secara manual.