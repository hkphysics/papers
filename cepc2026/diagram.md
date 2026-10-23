block-beta
  columns 5
  classDef tight padding:0;
  classDef label fill:none,stroke:none,padding:0
  block:presentation:4
    columns 4
    browser["Browser / UI"]
  end
  presLabel["Presentation layer"]:1
  style presentation 
  block:proxy:4
    columns 1
    traefik["Traefik reverse proxy"]:1
  end
  proxyLabel["Proxy / Auth layer"]:1

  block:computation:4
    columns 2
    jupyter["Jupyter"] openwebui["OpenWebUI"]
  end
  compLabel["Computation layer"]:1  

  block:dispatch:4
    columns 2
    litellm["Litellm"]:1 searxng["SearXNG"]:1
  end
  dispLabel["Dispatch layer"]:1  

  block:agentic:4
    columns 3
    openclaw["OpenClaw"] hermes["Hermes"] pi["Pi"]
  end
  agentLabel["Agentic layer"]:1

  block:model:4
    columns 2
    ollama["Local Ollama"] cloud["Cloud LLMs"] 
  end
  modelLabel["Model / LLM layer"]:1


  class presLabel,dispLabel,agentLabel,modelLabel,compLabel,proxyLabel label