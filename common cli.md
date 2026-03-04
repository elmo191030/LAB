hf download nvidia/Qwen3-14B-FP4 \
  --local-dir ~/elmo-models/Qwen3-8B-FP4


請問你知道珍珠奶茶嗎
比較有名的是哪幾家


nvidia/Qwen3-8B-FP4
nvidia/Qwen3-14B-FP4
nvidia/Qwen3-32B-FP4
openai/gpt-oss-20b
openai/gpt-oss-120b
unsloth/Qwen3-30B-A3B-Base-bnb-4bit

MODEL_ID="Qwen/Qwen2.5-1.5B-Instruct" docker compose up -d --force-recreate vllm



MODEL_ID="nvidia/Qwen3-8B-FP4" docker compose up -d --force-recreate vllm
MODEL_ID="nvidia/Qwen3-14B-FP4" docker compose up -d --force-recreate vllm
MODEL_ID="nvidia/Qwen3-32B-FP4" docker compose up -d --force-recreate vllm
MODEL_ID="openai/gpt-oss-20b" docker compose up -d --force-recreate vllm
MODEL_ID="openai/gpt-oss-120b" docker compose up -d --force-recreate vllm
MODEL_ID="Qwen/Qwen2.5-1.5B-Instruct" docker compose up -d --force-recreate vllm


python3 bench_v3.py



docker exec -it vllm hf download Qwen/Qwen2.5-32B-Instruct

Qwen/Qwen2.5-1.5B-Instruct
Qwen/Qwen2.5-7B-Instruct
Qwen/Qwen2.5-14B-Instruct
Qwen/Qwen2.5-32B-Instruct



MODEL_ID=nvidia/Qwen3-14B-FP4 docker compose up -d

docker compose down



huggingface-cli download nvidia/Qwen3-8B-FP4  
--local-dir /root/.cache/huggingface/Qwen3-8B-FP4 
--local-dir-use-symlinks False


ls -lh /root/.cache/huggingface/Qwen3-8B-FP4


curl http://localhost:8000/v1/chat/completions \
-H "Content-Type: application/json" \
-d '{
    "model": "Qwen/Qwen2.5-1.5B-Instruct",
    "messages": [{"role": "user", "content": "12*17"}],
    "max_tokens": 500
}'


