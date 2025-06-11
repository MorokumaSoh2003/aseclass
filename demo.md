# 研究

## 目次

- 研究概要
- CUDAのコード例
- GPUの画像

## 研究概要

私は、GPUの高い並列処理能力を活用し、量子化学計算の高速化に関する研究に取り組んでいます。具体的には、C/C++を基盤とするGPUコンピューティングのための統合開発環境であるCUDAを用いて、量子化学計算における計算タスクをGPU上で効率的に並列実行するプログラムの設計・実装を行い、計算速度の大幅な向上を目指しています。

## CUDAのコード例
```
__global__ void MatAdd(float *A, float *B, float *C, int N) {
    int index = blockDim.x * blockIdx.x + threadIdx.x;

    if(index < N) {
        C[index] = A[index] + B[index];
    }
}
```

## GPUの画像

![](https://th.bing.com/th/id/OIP.T8uv_XQXkd2K4QWcct_pMgHaEj?w=289&h=180&c=7&r=0&o=7&dpr=1.5&pid=1.7&rm=3)