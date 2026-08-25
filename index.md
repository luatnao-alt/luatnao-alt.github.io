---
layout: default
title: "Kho Kiến Thức & Kho Kiến Thức & Tra Cứu Tri Thức Pháp Luật Việt Nam - LuatNao.vn"
description: "Kho lưu trữ & Tra cứu kiến thức pháp luật Việt Nam thời gian thực. Hệ thống AI phân tích và đối chiếu đa tầng Nghị định, Thông tư hiện hành."
---

<!-- ── 상단 커스텀 스타일 ── -->
<style>
  :root {
    --brand-primary: #2563eb;
    --brand-dark: #0f172a;
    --brand-gradient: linear-gradient(135deg, #1e40af 0%, #3b82f6 100%);
    --card-bg: #ffffff;
    --card-border: #e2e8f0;
    --text-main: #0f172a;
    --text-muted: #64748b;
  }

  /* 글로벌 네비게이션 헤더 */
  .archive-nav {
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
    gap: 14px;
    padding: 14px 20px;
    background: #0f172a;
    border-radius: 14px;
    margin-bottom: 24px;
    box-shadow: 0 4px 18px rgba(0, 0, 0, 0.15);
    border: 1px solid rgba(255, 255, 255, 0.08);
  }
  .archive-brand {
    display: flex;
    align-items: center;
    gap: 10px;
    text-decoration: none;
  }
  .archive-brand-logo {
    width: 32px;
    height: 32px;
    object-fit: contain;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgba(37, 99, 235, 0.3);
  }
  .archive-brand-text {
    font-size: 16px;
    font-weight: 800;
    color: #ffffff;
    letter-spacing: -0.02em;
  }
  .archive-brand-badge {
    font-size: 10px;
    font-weight: 700;
    background: rgba(59, 130, 246, 0.2);
    color: #60a5fa;
    border: 1px solid rgba(59, 130, 246, 0.4);
    padding: 2px 6px;
    border-radius: 4px;
    text-transform: uppercase;
  }
  .archive-nav-links {
    display: flex;
    align-items: center;
    gap: 8px;
    flex-wrap: wrap;
  }
  .archive-nav-link {
    color: #94a3b8;
    text-decoration: none;
    font-size: 13.5px;
    font-weight: 600;
    padding: 6px 12px;
    border-radius: 8px;
    transition: all 0.2s;
  }
  .archive-nav-link:hover, .archive-nav-link.active {
    color: #ffffff;
    background: rgba(255, 255, 255, 0.12);
  }
  .btn-launch-ai {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    background: linear-gradient(135deg, #2563eb 0%, #4f46e5 100%);
    color: #ffffff !important;
    text-decoration: none;
    font-size: 13px;
    font-weight: 700;
    padding: 8px 16px;
    border-radius: 8px;
    box-shadow: 0 2px 10px rgba(37, 99, 235, 0.4);
    transition: all 0.2s;
  }
  .btn-launch-ai:hover {
    transform: translateY(-1px);
    box-shadow: 0 4px 16px rgba(37, 99, 235, 0.6);
  }

  /* 검색 및 필터 구획 */
  .search-section {
    background: #ffffff;
    border: 1px solid #e2e8f0;
    border-radius: 14px;
    padding: 20px;
    margin-bottom: 28px;
    box-shadow: 0 4px 20px -4px rgba(0, 0, 0, 0.05);
  }
  .search-input-wrap {
    position: relative;
    margin-bottom: 14px;
  }
  .search-input-wrap input {
    width: 100%;
    box-sizing: border-box;
    padding: 13px 16px 13px 44px;
    font-size: 15px;
    border: 2px solid #cbd5e1;
    border-radius: 10px;
    outline: none;
    transition: border-color 0.2s;
  }
  .search-input-wrap input:focus {
    border-color: #2563eb;
    box-shadow: 0 0 0 3px rgba(37, 99, 235, 0.15);
  }
  .search-icon {
    position: absolute;
    left: 14px;
    top: 50%;
    transform: translateY(-50%);
    font-size: 18px;
    color: #94a3b8;
  }
  .filter-chips {
    display: flex;
    gap: 8px;
    flex-wrap: wrap;
    align-items: center;
  }
  .filter-chip {
    background: #f1f5f9;
    border: 1px solid #e2e8f0;
    color: #475569;
    font-size: 12.5px;
    font-weight: 600;
    padding: 6px 12px;
    border-radius: 20px;
    cursor: pointer;
    transition: all 0.15s;
    user-select: none;
  }
  .filter-chip:hover {
    background: #e2e8f0;
    color: #0f172a;
  }
  .filter-chip.active {
    background: #2563eb;
    border-color: #2563eb;
    color: #ffffff;
  }
  .search-count-bar {
    margin-top: 12px;
    font-size: 12.5px;
    color: #64748b;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 8px;
  }

  /* 카드 그리드 */
  .posts-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
    gap: 18px;
    margin-bottom: 40px;
  }
  .post-card {
    background: #ffffff;
    border: 1px solid #e2e8f0;
    border-radius: 12px;
    padding: 18px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    transition: all 0.2s cubic-bezier(0.16, 1, 0.3, 1);
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.04);
  }
  .post-card:hover {
    transform: translateY(-3px);
    border-color: #93c5fd;
    box-shadow: 0 10px 24px -4px rgba(37, 99, 235, 0.12);
  }
  .post-card-meta {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 10px;
  }
  .post-category-badge {
    background: #eff6ff;
    color: #1d4ed8;
    border: 1px solid #bfdbfe;
    font-size: 11px;
    font-weight: 700;
    padding: 3px 8px;
    border-radius: 6px;
    text-transform: uppercase;
  }
  .post-date {
    font-size: 12px;
    color: #94a3b8;
  }
  .post-card-title {
    font-size: 16px;
    font-weight: 700;
    color: #0f172a;
    line-height: 1.45;
    margin-bottom: 8px;
  }
  .post-card-title a {
    color: inherit;
    text-decoration: none;
  }
  .post-card-title a:hover {
    color: #2563eb;
  }
  .post-card-desc {
    font-size: 13px;
    color: #64748b;
    line-height: 1.55;
    margin-bottom: 14px;
    display: -webkit-box;
    -webkit-line-clamp: 2;
    -webkit-box-orient: vertical;
    overflow: hidden;
  }
  .post-card-tags {
    display: flex;
    gap: 4px;
    flex-wrap: wrap;
    margin-bottom: 12px;
  }
  .post-tag {
    font-size: 10.5px;
    color: #64748b;
    background: #f8fafc;
    border: 1px solid #e2e8f0;
    padding: 2px 6px;
    border-radius: 4px;
  }
  .post-card-footer {
    display: flex;
    align-items: center;
    justify-content: space-between;
    border-top: 1px solid #f1f5f9;
    padding-top: 10px;
    margin-top: auto;
  }
  .post-card-link {
    font-size: 13px;
    font-weight: 600;
    color: #2563eb;
    text-decoration: none;
  }
  .post-card-link:hover {
    text-decoration: underline;
  }

  /* 하단 푸터 & 방문자 카운터 */
  .archive-footer {
    margin-top: 48px;
    padding: 28px 20px;
    background: #0f172a;
    border-radius: 14px;
    color: #94a3b8;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    gap: 16px;
    border: 1px solid rgba(255, 255, 255, 0.08);
  }
  .visitor-counter-bar {
    display: flex;
    align-items: center;
    gap: 12px;
    flex-wrap: wrap;
    justify-content: center;
    background: rgba(255, 255, 255, 0.05);
    padding: 8px 16px;
    border-radius: 24px;
    border: 1px solid rgba(255, 255, 255, 0.1);
  }
  .no-results-box {
    grid-column: 1 / -1;
    text-align: center;
    padding: 48px 20px;
    background: #f8fafc;
    border: 1px dashed #cbd5e1;
    border-radius: 12px;
    display: none;
  }
</style>

<!-- ── 1. 상단 글로벌 네비게이션 헤더 (공식 로고 탑재) ── -->
<nav class="archive-nav">
  <a href="https://luatnao-alt.github.io/" class="archive-brand">
    <img src="https://luatnao-alt.github.io/assets/images/logo.png" alt="LuatNao.vn Logo" class="archive-brand-logo" onerror="this.onerror=null; this.src='https://luatnao-alt.github.io/logo.png';" />
    <span class="archive-brand-text">LuatNao.vn</span>
    <span class="archive-brand-badge">Archive</span>
  </a>

  <div class="archive-nav-links">
    <a href="#" class="archive-nav-link active" onclick="setCategoryFilter('all', this); return false;">🏠 Tất cả (전체)</a>
    <a href="#" class="archive-nav-link" onclick="setCategoryFilter('giao-thong', this); return false;">🚗 Giao thông (교통)</a>
    <a href="#" class="archive-nav-link" onclick="setCategoryFilter('lao-dong', this); return false;">💼 Lao động (노동)</a>
    <a href="#" class="archive-nav-link" onclick="setCategoryFilter('bat-dong-san', this); return false;">🏢 Bất động sản (부동산)</a>
  </div>

  <a href="https://luatnao.vn" target="_blank" rel="noopener" class="btn-launch-ai">
    ⚡ Tra Cứu Tri Thức LuatNao →
  </a>
</nav>

<!-- ── 2. 상단 검색 및 퀵 태그 필터 바 ── -->
<div class="search-section">
  <div class="search-input-wrap">
    <span class="search-icon">🔍</span>
    <input type="text" id="liveSearchInput" placeholder="Tìm kiếm theo từ khóa, mức phạt, điều luật, câu hỏi... / 키워드, 벌금, 질문 검색..." oninput="handleLiveSearch()" />
  </div>

  <div class="filter-chips">
    <span style="font-size: 12px; font-weight: 700; color: #475569; margin-right: 4px;">🏷️ Lọc nhanh:</span>
    <span class="filter-chip active" onclick="setTagFilter('all', this)">Tất cả (전체)</span>
    <span class="filter-chip" onclick="setTagFilter('phap-luat-viet-nam', this)">#PhápLuậtVN</span>
    <span class="filter-chip" onclick="setTagFilter('traffic', this)">#GiaoThông</span>
    <span class="filter-chip" onclick="setTagFilter('speed-fine', this)">#MứcPhạtQuáTốcĐộ</span>
    <span class="filter-chip" onclick="setTagFilter('demerit-points', this)">#ĐiểmTrừGPLX</span>
    <span class="filter-chip" onclick="setTagFilter('lao-dong', this)">#HợpĐồngLaoĐộng</span>
  </div>

  <div class="search-count-bar">
    <span id="searchResultCount">Hiển thị tất cả bài viết</span>
    <span>⚡ Cập nhật tự động thời gian thực từ LuatNao AI</span>
  </div>
</div>

<!-- ── 3. 법률 Q&A 카드 그리드 ── -->
<div class="posts-grid" id="postsGrid">
{% for post in site.posts %}
  <article class="post-card" 
    data-title="{{ post.title | downcase | escape }}"
    data-desc="{{ post.description | default: post.excerpt | strip_html | downcase | escape }}"
    data-categories="{{ post.categories | join: ' ' | downcase }}"
    data-tags="{{ post.tags | join: ' ' | downcase }}"
  >
    <div>
      <div class="post-card-meta">
        <span class="post-category-badge">{{ post.categories | first | default: "Legal-QA" }}</span>
        <span class="post-date">📅 {{ post.date | date: "%Y-%m-%d" }}</span>
      </div>

      <h3 class="post-card-title">
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>

      <div class="post-card-desc">
        {{ post.description | default: post.excerpt | strip_html | truncate: 120 }}
      </div>

      {% if post.tags.size > 0 %}
        <div class="post-card-tags">
          {% for tag in post.tags limit:4 %}
            <span class="post-tag">#{{ tag }}</span>
          {% endfor %}
        </div>
      {% endif %}
    </div>

    <div class="post-card-footer">
      <a href="{{ post.url | relative_url }}" class="post-card-link">Đọc chi tiết bài viết →</a>
      <a href="https://luatnao.vn" target="_blank" rel="noopener" style="font-size: 11.5px; color: #64748b; text-decoration: none;">🔍 Tra Cứu Thêm</a>
    </div>
  </article>
{% endfor %}

  <!-- 검색 결과 없음 안내 -->
  <div class="no-results-box" id="noResultsBox">
    <div style="font-size: 32px; margin-bottom: 8px;">🔍</div>
    <h4 style="margin: 0 0 6px 0; color: #0f172a; font-size: 16px;">Không tìm thấy bài viết phù hợp</h4>
    <p style="margin: 0 0 16px 0; color: #64748b; font-size: 13px;">일치하는 Q&A 게시글이 없습니다. LuatNao.vn에서 LuatNao.vn에서 최신 법령 조항을 검색해 보세요!</p>
    <a href="https://luatnao.vn" target="_blank" rel="noopener" class="btn-launch-ai" style="display: inline-flex;">
      ⚡ Tra Cứu Tại LuatNao.vn
    </a>
  </div>
</div>

<!-- ── 4. 하단 푸터 & 실시간 방문자 카운터 (Visitor Counter) ── -->
<footer class="archive-footer">
  <div style="display: flex; align-items: center; gap: 8px;">
    <img src="assets/images/logo.png" alt="LuatNao.vn" style="width: 24px; height: 24px; object-fit: contain;" onerror="this.onerror=null; this.src='logo.png';" />
    <strong style="color: #ffffff; font-size: 15px;">LuatNao.vn Legal Intelligence</strong>
  </div>

  <p style="margin: 0; font-size: 12.5px; max-width: 540px; line-height: 1.6;">
    Hệ thống lưu trữ và tra cứu kiến thức pháp luật Việt Nam tự động hóa. Cập nhật liên tục theo các Nghị định, Thông tư mới nhất.
  </p>

  <!-- 실시간 방문자 카운터 위젯 배지 -->
  <div class="visitor-counter-bar">
    <span style="font-size: 12.5px; color: #cbd5e1; font-weight: 700;">📊 LuatNao Views:</span>
    <img src="https://komarev.com/ghpvc/?username=luatnao-alt&label=TOTAL+VIEWS&color=2563eb&style=flat-square" alt="Total Pageviews" style="vertical-align: middle; border-radius: 4px;" />
    <img src="https://api.visitorbadge.io/api/combined?path=https%3A%2F%2Fluatnao-alt.github.io&label=VISITORS&labelColor=%230f172a&countColor=%232563eb&style=flat-square" alt="Live Visitors" style="vertical-align: middle; border-radius: 4px;" />
  </div>

  <div style="font-size: 11.5px; color: #64748b; margin-top: 6px;">
    © 2026 <strong><a href="https://luatnao.vn" target="_blank" rel="noopener" style="color: #60a5fa; text-decoration: none;">LuatNao.vn</a></strong>. All rights reserved. Powered by GitHub Pages & Legal AI.
  </div>
</footer>

<!-- ── 실시간 클라이언트 검색 스크립트 ── -->
<script>
  let currentCategory = 'all';
  let currentTag = 'all';

  function handleLiveSearch() {
    const query = (document.getElementById('liveSearchInput').value || '').toLowerCase().trim();
    const cards = document.querySelectorAll('.post-card');
    let visibleCount = 0;

    cards.forEach(card => {
      const title = card.getAttribute('data-title') || '';
      const desc = card.getAttribute('data-desc') || '';
      const categories = card.getAttribute('data-categories') || '';
      const tags = card.getAttribute('data-tags') || '';

      const matchesQuery = !query || title.includes(query) || desc.includes(query) || tags.includes(query);
      const matchesCategory = currentCategory === 'all' || categories.includes(currentCategory) || tags.includes(currentCategory) || title.includes(currentCategory);
      const matchesTag = currentTag === 'all' || tags.includes(currentTag) || categories.includes(currentTag);

      if (matchesQuery && matchesCategory && matchesTag) {
        card.style.display = 'flex';
        visibleCount++;
      } else {
        card.style.display = 'none';
      }
    });

    const noResults = document.getElementById('noResultsBox');
    const countBar = document.getElementById('searchResultCount');

    if (visibleCount === 0) {
      if (noResults) noResults.style.display = 'block';
      if (countBar) countBar.innerText = 'Không có kết quả nào (검색 결과 없음)';
    } else {
      if (noResults) noResults.style.display = 'none';
      if (countBar) countBar.innerText = 'Hiển thị ' + visibleCount + ' / ' + cards.length + ' bài viết (' + visibleCount + '개 표시 중)';
    }
  }

  function setCategoryFilter(cat, elem) {
    currentCategory = cat;
    document.querySelectorAll('.archive-nav-link').forEach(el => el.classList.remove('active'));
    if (elem) elem.classList.add('active');
    handleLiveSearch();
  }

  function setTagFilter(tag, elem) {
    currentTag = tag;
    document.querySelectorAll('.filter-chip').forEach(el => el.classList.remove('active'));
    if (elem) elem.classList.add('active');
    handleLiveSearch();
  }
</script>
