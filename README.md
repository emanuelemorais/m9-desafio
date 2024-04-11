# Ponderada - 1 Bilhão de Linhas em Zig - Emanuele Morais

## Como Executar

- Baixe o seu executável do Zig

- Após baixar o executável, dentro do diretório `m9-desafio`, execute o comando abaixo para compilar.

```
zig build -Doptimize=ReleaseFast
```

- Para criar um arquivo TXT com um bilhão de linhas execute os comandos abaixo em sequência.
> [!NOTE]
> Isso irá criar uma arquivo de aproximandamente 12GB e irá demorar alguns minutos

```
run-create-sample
```
```
./zig-out/bin/run-create-sample 1000000000
```

- Por fim execute o comando abaixo para ver o tempo de execução
```
time ./zig-out/bin/1brc-zig measurements.txt
```

## Resultados 

**Máquina:** MacBook Air (M2, 2022) - Memória unificada de 8 GB, CPU de 8 núcleos (4 de desempenho e 4 de eficiência), GPU de 8 núcleos

**Tempo de execução**: 36.96x

```./zig-out/bin/1brc-zig measurements.txt  36.96s user 12.64s system 179% cpu 27.653 total```

![alt text](<Screenshot 2024-04-11 at 18.10.56.png>)

