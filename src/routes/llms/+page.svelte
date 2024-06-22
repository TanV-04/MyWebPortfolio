<div class="py-6">
  <h1 class="text-center text-3xl font-bold">
    Can Green Coding Bridge the Gap Between LLMs and a Healthy Planet?
  </h1>
</div>

<div class="prose px-4 mx-auto leading-loose">
  <p>
    Did you know that training a single Large Language Model (LLM) can emit as
    much CO2 as driving a car around the Earth’s equator approximately 300
    times? When you’re scrolling through Instagram, liking posts, and sharing
    reels without a thought, behind the scenes, each interaction is fuelled by
    massive data centres running around the clock, emitting carbon emissions,
    that are often overlooked. It’s a staggering reality about LLMs as they’ve
    taken the world by storm.
  </p>

  <p>
    These models have the incredible ability to process huge amounts of data,
    but there's a downside: training and maintaining them requires a massive
    amount of computational power, which leads to a large trail of carbon
    emissions that goes unnoticed. For example, a single query on the very
    popular LLM, ChatGPT, can consume up to 100 times more energy than a Google
    search. This is just the tip of the iceberg.
  </p>

  <p>
    That’s where green coding steps in, an emerging practice advocating for
    sustainable software development practices by optimizing algorithms,
    designs, and hardware for energy efficiency. This article delves into the
    potential of green coding to address environmental concerns of LLMs, paving
    the way for a future where machine learning and a healthy planet coexist.
  </p>

  <h2><strong>Understanding the Environmental Impact of LLMs:</strong></h2>
  <ul>
    <li>
      Given the rapid advancements in AI, it is crucial to take into
      consideration the factors defining the carbon footprint of these
      technologies:
      <ul>
        <li>
          - Hardware: When it comes to the energy consumption of ML models, the
          efficiency and type of hardware, including GPUs, really matter. While
          newer technology can help with energy demands, the high requirements
          for training large models may outweigh the benefits.
        </li>
        <li>
          - Training data: It’s important to remember that larger datasets can
          increase the carbon footprint and use more energy for processing.
          That's why it's crucial to optimize the dataset size and complexity to
          help maintain sustainability.
        </li>
        <li>
          - Model architecture: Creating larger and more complex networks
          requires more energy. The energy consumption is also higher when a
          model trains for a long time. Simplifying the architecture of these
          models can help save a lot of energy without affecting their
          performance.
        </li>
        <li class="point1">
          - Location of data centres: Data centres that use renewable energy
          have a smaller impact on the environment compared to those that rely
          on non-renewable sources. This shows how important it is to choose the
          right location for data centres to reduce their environmental
          footprint.
        </li>
      </ul>
    </li>
  </ul>

  <p>
    The environmental cost of training and operating LLMs becomes very clear by
    examining case studies that illustrate their carbon emissions and energy
    use. Take a look at the box plot given below as it describes CO2 emitted in
    grams corresponding to each ML task.
  </p>

  <img
    src="src\images\carbonEmitted.png"
    style="float: right; margin-left: 20px; width: 50%;"
  />

  <p>
    The training of GPT-4, one of the most advanced language models to date,
    required resources that led to significant environmental impacts. For
    example, the carbon footprint generated during its development is comparable
    to the emissions from driving a gas-powered car nearly 29 million kilometres
    or powering 1,300 homes for a year! Just a day’s operation of GPT-3 alone
    emits around 8.4 tons of CO2 per year! One may not notice it, but beneath
    the surface lies an unseen threat to the environment.
  </p>

  <p>
    The graph to the right presents a staggering estimation of the number of
    homes that can be powered by just training these LLMs and the numbers are
    eye-opening.
  </p>

  <img
    src="src\images\numberOfHomes.png"
    style="float: right; margin-left: 20px;  width:50%"
  />

  <p>
    Additionally, beyond carbon emissions, disinformation and transparency risks
    pose significant challenges to maintaining the environmental balance. The
    problem is that it is very difficult to assess gas emissions due to a lack
    of transparency from tech companies who own these LLMs. Recent insights
    gleaned that training BERT on a GPU is comparable to a cross-country flight,
    while BLOOM’s training emits as much CO2 as 30 flights between London and
    New York, and GPT-3’s training equals 500 tons of CO2 emissions (nearly 600
    flights!). Furthermore, OpenAI recently disclosed that $700,000 was spent on
    running ChatGPT, which wasn’t even a sustainable model from a business
    perspective!
  </p>

  <h2><strong>Introduction to Green Coding:</strong></h2>
  <p>
    Green coding offers a multi-faceted approach to tackling the environmental
    challenge of LLMs. While its definition states that it is the degree of
    eco-friendliness of the model considering the specific problems, gauged
    against selected sustainability metrics, its scope extends far beyond this
    textbook definition.
  </p>

  <ul>
    <li>
      Some of the key strategies involve:
      <ul>
        <li>
          - Hardware Design Optimization: Leverage specialized hardware
          accelerators like GPUs or Tensor Processing Units (TPUs) or explore
          cloud platforms offering renewable energy sources.
        </li>
        <li>
          - Software Design Optimization: Involves practices like code
          refactoring, memory optimization, and minimizing redundant
          computations.
        </li>
        <li class="point2">
          - Algorithm Optimization: Involves techniques like data pruning,
          quantization, and model compression.
        </li>
      </ul>
    </li>
  </ul>

  <p>
    The following metrics provide a comprehensive framework to evaluate the
    sustainability of generated codes:
  </p>

  <ul>
    <li>
      - Code correctness: Ensure the generated code is correct because incorrect
      code requires additional effort to be corrected, making it unsustainable.
    </li>
    <li>- Runtime: Longer runtimes may indicate inefficiencies in the code.</li>
    <li>
      - Memory: Efficient memory usage is crucial for sustainability, especially
      in systems with limited resources.
    </li>
    <li>
      - FLOPs (Floating-Point Operations): These mathematical calculations
      provide insights into how optimized an algorithm is by reducing the
      expensive computations required to solve a certain problem.
    </li>
    <li>
      - Energy consumption: Lower energy consumption indicates a more
      sustainable and efficient code.
    </li>
  </ul>
  <br />

  <h2>
    <strong> Ongoing Efforts and Initiatives in Green Coding for LLMs: </strong>
  </h2>

  <ul>
    <li>
      There aren’t many real-world examples today, but the following initiatives
      are laying the groundwork where green coding becomes an integral part of
      LLM development and deployment:
      <ul>
        <li>
          - Google AI and DeepMind are collaborating on research to optimize
          models and improve hardware efficiency for LLMs. Their goal is to
          reduce energy consumption during training, and they’ve achieved a 40%
          reduction in energy usage for cooling by developing more efficient
          servers and cooling methods for their data centres.
        </li>
        <li>
          - The MLPerf Benchmark sets standardized benchmarks for measuring the
          performance and the efficiency of ML models.
        </li>
        <li>
          - Major cloud providers like Google and Microsoft are using renewable
          energy to power their data centres, which reduces the carbon footprint
          of LLMs trained and deployed on these platforms.
        </li>
      </ul>
    </li>
  </ul>

  <br />
  <h2>
    <strong> Conclusion: </strong>
  </h2>

  <p>
    The rise of LLMs has introduced an era of innovation and endless
    possibilities, but like all powers, it came with a hidden cost – a growing
    carbon footprint. As we explored, training and operating these models
    consumed vast amounts of energy, leaving a trail of carbon emissions. The
    challenges we face are real. As a community of developers, researchers, and
    users, it's important to adopt and promote environmentally-friendly coding
    practices. This means raising awareness, fostering collaboration, and
    integrating green coding principles into our daily routines, as well as
    exploring ways to incorporate them into LLM development workflows. Together,
    we can bridge the gap between AI and a healthy planet by taking action
    today, and ensure that LLMs continue to evolve by reducing their significant
    contribution to the existing trail of environmental destruction.
  </p>
</div>

<style>
  .prose {
    font-weight: bold;
    margin-bottom: 40px;
  }

  .prose p {
    text-indent: 3em;
    margin-bottom: 20px;
  }

  .point1, .point2 {
    margin-bottom: 14px;
  }

  img {
    border-radius: 6px;
    border-style: double;
    border-width: 3px;
  }

</style>
